README.md
README.md must include:

    A short summary of what you learned about AI and self-reliance.
# AI is a useful tool to help make work easier and faster and not to replace human thinking. It can be abused when over dependence occur.

    Your main insight about using AI ethically as a coder.
# Privacy and security of data. AI as an aid tool not answer generator. Using AI ethically.
    One paragraph describing how you plan to apply these principles in future quests.
# Applying AI to understand the how and why not answer generation. Using and applying all ethical standards with AI and much as data security.

---

quest00/ex00_reflection.md
Exercise 0: Honest Reflection on AI Use

Objective: Understand your current relationship with AI in coding and learning.

    Write short, honest answers to these questions:

        How have you used AI for coding so far?
            Answer: Yes, I have. During the piscine (trials), i used AI for learning golang-go.

        Do you usually try problems yourself first?
            Answer: I do, most times but not all the time. 

        Can you explain code you've submitted without AI's help?
            Answer: As a beginner, i think the first code i submitted without AI's help was printing "Hello World!" using go-language.

        What would happen if AI was unavailable during an exam or job test?
            Answer: AI is important and very useful in learning. Most traditional exams wouldn't allow the use of AI during exam or job test. This doesn't make it any easier. However, unavailability of AI during exam or job test especially in coding or programming might result in poor result outcomes. Although, AI shouldn't be used as a replacement for learning and studying, it is however important.

    Identify your current pattern:

        Learner A: uses AI as an answer generator.

        Learner B: uses AI as a learning amplifier.
            Answer: Learner B
            
    Write a short paragraph describing where you are today and what type of learner you want to become.
            Answer: Few months ago, I didn't know anything about programming. No class teacher or instructor, no pressures, just the internet and AI. Today, i'm in a much better place than i know i used to be. I want to be the learner who uses AI as a learning amplifier not just an answer generator. I want to understand the why, what, where, how and when.

            ---

            quest00/ex01_palindrome.md
            Exercise 1: The Palindrome Challenge

Objective: Experience the difference between using AI as a shortcut and using it as a learning tool.
Step 1 - Do it yourself

    Write pseudocode for a function that checks if a string is a palindrome.
        Answer: // A palindrome is a word, phrase, number or sentence that can be read forward or backward and means the same thing.//
        Pseudocode:
        input = ('s')
        s = "dad"
        if isPalindrome 'true'
        else: "false"
        print(s)

    Implement your solution in Python.
        Answer: 
        def is_Palindrome (str):
            if str == str [::-1]:
                return True
            else: return False

        word = "dad"
        if is_Palindrome(word):
            print(f"'{word} is a Palindrome")
        else: print(f"'{word} is not a Palindrome")

    Test with examples like "racecar", "hello", and "A man a plan a canal Panama".
        Answer: 
        def is_Palindrome (str):
            if str == str [::-1]:
                return True
            else: return False

word = "racecar"
if is_Palindrome(word):
        print(f"'{word} is a Palindrome")
else: print(f"'{word} is not a Palindrome")

word = "hello"
if is_Palindrome(word):
        print(f"'{word} is a Palindrome")
else: print(f"'{word} is not a Palindrome")

word = "A man a plan a canal Panama"
if is_Palindrome(word):
        print(f"'{word} is a Palindrome")
else: print(f"'{word} is not a Palindrome")

    Add comments explaining your reasoning.
        Answer: // A palindrome can be read after running backwards. I used the slice trick for palindrome on python to return every string and check if it's a palindrome.


Step 2 - Use AI to learn

Now that your function works, use AI to go deeper:
"I wrote a palindrome function. Here's my code:
[insert your code]

What's the time complexity?
    Answer: The time complexity = O(n). 
What edge cases might I miss?
    Answer: Case sensitivity, punctuations and spaces, single string, empty character.
Are there better approaches?"
    Answer: As suggested by AI
        For interviews or production code, normalization + two pointers is the most robust.


Step 3 - Reflection

    What did you learn from solving it before asking AI?
        Answer: I first tried to define and understand the meaning and application of pseudocode and palindrome. The knowledge gained helped me with understand what needed to be done. AI was used to fix bugs and identify areas of improvement and deep learning.

    How is your understanding different now?
        Answer: Understanding the basics is key to solving these problems.

    Could you now write similar functions (e.g., reverse a string) without help?
        Answer: yes!!!

---

quest00/ex02_variations.md
Exercise 2: Strengthening Through Variations

Objective: Extend your solution and practice independent problem-solving.

    Modify your palindrome function to:

        Ignore spaces and punctuation.
            Answer:
def is_Palindrome (str):
            if str == str [::-1]:
                return True
            else: return False

word = "dad"
if is_Palindrome(word):
        print(f"'{word} is a Palindrome")
else: print(f"'{word} is not a Palindrome")

        Be case-insensitive.
            Answer: I used the character 'dad' instead of 'Dad".

        Return the position where the string stops being a palindrome (if not one).


    After your first attempt, ask AI:

"I modified my palindrome function to handle more cases.
Did I miss anything? Can it be more efficient?"
        Answer: 
        def is_palindrome(s):
    # Step 1: Normalize the string
    # Keep only alphanumeric characters and convert to lowercase
    cleaned = ''.join(char.lower() for char in s if char.isalnum())

    # Step 2: Use two pointers to compare characters
    left = 0
    right = len(cleaned) - 1

    while left < right:
        # If characters do not match, it's not a palindrome
        if cleaned[left] != cleaned[right]:
            return False

        # Move pointers inward
        left += 1
        right -= 1

    # If all characters matched
    return True

    Reflect on what AI added that you didn't consider initially.
            Answer: Normalization and two pointer comparison.

---

quest00/ex03_fairness_contract.md
Objective: Define your personal rules for ethical AI use in learning.

Create a markdown file fairness_contract.md with three sections:

## I will use AI when:

    I have tried solving a problem myself.

    I need to understand why something works.

    I want to explore alternative approaches.

## I will NOT use AI when:

    I haven't tried the problem on my own.

    I am completing an exam or assessment.

    I am still learning fundamental concepts.

## I know I'm using AI fairly when:

    I can explain my code without AI's help.

    I could solve a similar problem independently.

    I feel more confident in my own understanding.

Sign and date your contract.

# Ofuru Prince Solomon
# pofuru
# 10-02-2026

---

quest00/ex04_scenarios.md
Exercise 4: Real-World Scenarios

Objective: Understand the real risks of over-reliance on AI.

Answer these three scenarios in a short markdown file:

    Interview: You're asked to explain a caching system design. What happens if you've always relied on AI to design systems?
        Answer: You'll not be able to explain.

    Production Bug: At 2 AM, you must debug code generated by AI months ago - but AI is offline. Can you fix it?
        Answer: I'm willing to try.

    New Technology: A new library is released, and AI hasn't been trained on it yet. How do you learn it?
        Answer: by practicing and learning from resources.

Reflection: Write one paragraph explaining how using AI fairly today prepares you for real-world challenges like these.
    Answer: Using AI fairly prepares me for the real-world challenges and its complexities. It's easy use tool and good source of learning not just to generate answers. In tech, health, agro, and businesses, it is effectively changing how we see the world.

---

quest00/ex05_irreplaceable_skills.md
Exercise 5: Building Irreplaceable Skills

Objective: Identify the human skills that separate good coders from AI users.

Rate yourself (1–5) in each skill and plan improvements:
| Skill | Description | Rating | Improvement Plan |
| ----- | --------- | ----- | ------------- |
Problem Decomposition | Breaking down problems logically | 4/5 | Take notes of each word i don't understand |	
Systems Thinking | Understanding how components interact | 3/5	| Seeking for simplier or basic explanations |
Critical Evaluation | Knowing when code is wrong or inefficient | 3/5 | payign attention to details
Debugging Mindset | Investigating unexpected behavior | 4/5 | spending more time to understand what needs to be done
Conceptual Understanding | Knowing WHY, not just HOW | 4/5 | research and analysis

Choose your lowest-rated skill and write 3 specific actions you'll take this week to improve it without relying on AI.
        Answer: 1. Spend more time studying and understanding how components interact.
                2. Trusting my instincts more
                3. Asking other resources other than AI


