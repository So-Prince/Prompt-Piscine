README.md
    What is a prompt?
#  A prompt is essentially the input you give a language model to get a response. Think of it as a question, instruction, or starting point that tells the AI what you want it to do.


    Anatomy of a prompt (system, user, assistant messages)
# How It All Works Together
    System: Sets the “rules of behavior” for the AI.
    User: Asks the question or gives instructions.
    Assistant: Provides previous responses to maintain context in a conversation.


    Zero-shot vs few-shot prompting
# Tip: 
    Few-shot prompting is like saying:
        "Here’s how to do it—now do a similar task."
    Zero-shot is more like:
        "Please do this task based only on the instruction."


    Introduction to completions in ChatGPT / Playground
# Temperature and Top-p in parameter experimentation

    When using a language model like GPT, parameters such as temperature and top-p play a crucial role in controlling how creative, deterministic, or random the model’s outputs are. Let’s break them down carefully.

1. Temperature
Definition:
Temperature controls the randomness of the model's predictions by scaling the probabilities of the next token.


Low temperature (e.g., 0.0–0.3):
The model becomes more deterministic.
It favors the most likely next words, producing predictable, focused responses.
Good for tasks needing accuracy, like summarization or code generation.


Medium temperature (e.g., 0.5–0.7):
Balances creativity and coherence.
The output can include some novel or unexpected phrasing while staying logical.


High temperature (e.g., 0.8–1.2):
Produces highly diverse and creative outputs.
May introduce more errors or illogical statements, because lower-probability tokens are more likely to be chosen.


Example (temperature effect):
Prompt: “Write a short story about a cat in space.”

Temp 0.2 → “A cat floated in the spaceship, carefully monitoring the controls.”

Temp 0.8 → “A mischievous feline bounced between zero-gravity snacks and alien gadgets, meowing at the stars.”



2. Top-p (nucleus sampling)
Definition:
Top-p sampling chooses the next word from the smallest set of words whose cumulative probability is ≥ p.


Low top-p (e.g., 0.1–0.3):
The model picks from only the most likely options.
Similar to low temperature: outputs are conservative.


Medium top-p (e.g., 0.5–0.8):
Allows for a moderate level of creativity.
Balances probable words with some unexpected choices.


High top-p (e.g., 0.9–1.0):
Includes almost all possible words, even rare ones.
Generates very creative or surprising text, but can become nonsensical.


Example (top-p effect):
Prompt: “Finish the sentence: The dragon flew over the mountains and…”

Top-p 0.3 → “…landed in the valley.”

Top-p 0.9 → “…danced with the clouds, singing an ancient melody of fire and sky.”



3. Interaction Between Temperature and Top-p

Low temperature + low top-p: Very safe, predictable output.

High temperature + high top-p: Highly creative, unpredictable output.

Low temperature + high top-p: Can produce occasional surprises but still somewhat grounded.

High temperature + low top-p: Contradictory; can produce odd or repetitive choices because high randomness is constrained to few options.



✅ Key Takeaways
Temperature = “how much randomness per token”
Top-p = “which words are considered at all”
Adjusting them together allows you to fine-tune creativity vs. reliability.
For structured tasks, keep both low; for creative writing, increase one or both.

---

Ex0_Environment_and_Libraries.py
import sys
print(sys.version)

word = "Hello, World!"
print(word)

---

Ex1_Simple_prompt_writing.md
    Write a direct instruction prompt (e.g., “List three programming languages”).
# Summarize the duties of a professional doctor
    Write a question style prompt (e.g., “What are the benefits of Python for AI?”).
# What are the duties of a professional doctor?
    Compare how the model answers each type.
# The second answer aimed for comprehensive explanation, while the first aimed for brevity and clarity. The model adjusted tone, length, and depth based on the command word (“what are” vs. “summarize”).

---

Ex2_Instruction_refinement.md
    Start with a vague request like: “Tell me about AI.”
# Can a beginner start?
    Refine it step by step into a clear instruction, e.g.,

        “Explain AI in simple terms for beginners.”

        “Summarize the main AI techniques in 5 bullet points.”
# Can a beginner start coding? What are the basics of coding? How can a beginner succeed in coding? Explain coding in simple terms for beginners. Summarize the coding concept for beginners.
    Compare outputs and note differences.
# Vague request lack context. AI is unable to understand fully and give appropriate results. Nothing is learned.
# The second (refined) prompt tell AI exactly what we want. Full detailed and comprehensive explanation on the subject topic is given.

---

Ex3_Parameter_experimentation.md
   # PROMPT: what are the duties of a professional doctor?
   
    Use the same prompt with temperature = 0.2 and then with temperature = 0.9.

# Temperature = 0.2 (low randomness)
    “A professional doctor examines patients, diagnoses illnesses, prescribes treatments, monitors recovery, maintains medical records, and advises on preventive care. They follow ethical guidelines and collaborate with other healthcare professionals to ensure patient well-being.”

# Temperature = 0.9 (high randomness)
    “A professional doctor guides patients through health challenges, sometimes exploring unconventional therapies, advising them about nutrition and mental well-being, and occasionally pondering the mysteries of life while scribbling notes in the clinic.”


    Repeat with different top-p values (e.g., 0.5 vs 1).
# Temperature of 0.2 with Top-p(0.5)
    “A professional doctor examines patients, diagnoses illnesses, prescribes treatments, and monitors recovery. They maintain medical records and advise on preventive care.”
# Temperature of 0.2 with Top-p(1.0)
    “A professional doctor examines patients, prescribes treatments, diagnoses illnesses, and monitors patient progress. They also educate patients on healthy practices and preventive care.”
# Temperature of 0.9 with Top-p(0.5)
    “A doctor may wander through the hospital corridors, diagnosing strange ailments, advising patients about mysterious remedies, and sometimes debating whether the universe favors health or illness.”
# Temperature of 0.9 with Top-p(1.0)
    “Doctors dance through their clinics like wizards, mixing potions of care and advice, talking to cats that resemble patients, and pondering the secrets of the human heart while scribbling notes in rainbow ink.”


    Record how the style, randomness, and focus of responses change.
# Temperature of 0.2 with Top-p(0.5)
    style - formal, factual
    randomness - very low
    focus - highly focused on core duties
# Temperature of 0.2 with Top-p(1.0)
    style - formal, slightly more descriptive
    randomness - low
    focus - still focused on main responsibilities
# Temperature of 0.9 with Top-p(0.5)
    style - narrative, imaginative
    randomness - high
    focus - moderately related to doctor duties
# Temperature of 0.9 with Top-p(1.0)
    style - highly creative, whimsical
    randomness - very high
    focus - loose connection to real duties


        # NB
            Observations:
                Temperature Effects
                Low temperature (0.2) → text is predictable, formal, and professional.
                High temperature (0.9) → text becomes creative, metaphorical, and less factual.

                Top-p Effects
                Lower top-p (0.5) → limits word choices to the most probable, keeping output focused.
                Higher top-p (1.0) → allows rare words and unusual constructions, increasing creativity and randomness.

                Combined Effects
                Low temp + low/medium top-p → most accurate, structured, professional description.
                High temp + high top-p → almost story-like or fantastical, sometimes unrelated to actual duties.
                High temp + low top-p → can still produce odd phrasing but constrained; tends to repeat some terms.

