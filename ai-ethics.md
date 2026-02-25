Ex00_ai_ethics_coder.md
Exercise 00: Learning to Use AI Ethically as a Coder

Objective: Understand the fundamental difference between using AI to get answers vs. using AI to learn and develop irreplaceable skills.
Part A: The Critical Distinction

Read and reflect: AI can already code. It can generate functions, debug syntax, and implement algorithms in seconds. This means:

If your only skill is writing code that AI can write, you are already replaceable. The question is not whether to use AI. The question is how to use it.

    Write down your honest answers:

    How have you used AI for coding so far?
# I use AI for coding alot but responsibly.
    Do you ask AI for solutions before trying yourself?
# No!
    Can you explain code you've submitted without AI's help?
# Yes
    What would happen if AI was suddenly unavailable during an exam or interview?
# A lot of coder will not be able to pass.
    Identify your current pattern: Which learner are you now? Learner A: "AI is my answer generator"

    Asks: "Write a function that does X"

    Copies code without reading carefully

    Moves on once it works

    Cannot explain how the code works

Learner B: "AI is my learning amplifier"

    Attempts the problem first

    Asks: "Why does this approach work? What are the trade-offs?"

    Tests understanding by explaining concepts

    Uses AI to explore deeper, not to avoid thinking
# Learner B
    Write a brief paragraph: Where are you now, and where do you want to be?
# Currently, as a new developer, i'm interested in understanding the why and how of problems. I am not perfect in coding so i do use AI for deep learning. I want to grow in wisdom and get to a point where I can fully and independently solve tactical problems without assistant.
Part B: The Wrong Way vs. The Right Way

Challenge: Implement a simple function to check if a string is a palindrome.
# my challenge
## def is_Palindrome(str):
    cleaned = ''.join(char.lower() for char in str if char.isalnum())
    return cleaned == cleaned [::-1]

word = "Prince"
if is_Palindrome(word):
    print(f"'{word}' is a palindrome")
else:
    print(f"'{word}' is not a palindrome")

Track A — The Wrong Way (observe but DO NOT do this):

    Immediately ask AI for the function

    Copy the code

    Test it, submit it, move on

Why this fails: You learn nothing, can't handle variations, can't explain your code, and train yourself to be dependent.

Track B — The Right Way (DO THIS): Step 1: Attempt independently

    Write pseudocode for a palindrome check

    Implement your solution in Python

    Test with examples: racecar, hello, A man a plan a canal Panama

    Debug any issues yourself

    Add comments explaining your logic
# my logic is simple. attempt, implement, ask questions and redefine. this challenge helped to discover a simplier and perfect way of writing a any palindrome problem.

Step 2: Strategic AI use After you have a working solution, ask AI:

"I wrote a function to check palindromes. Here's my approach: [paste YOUR code]

    What's the time complexity?
# 0(n)
    What edge cases am I missing?
# Unicorn characters
    Alternatives and trade-offs?
# Alternative 1: Two-Pointer (More Memory Efficient)
# Trade-off: Slightly more complex.

    How does it perform on very long strings?"
# More efficient for large stringS

Step 3: Reflection

    What did you learn by struggling first?
# It doesn't mean failure.
    How is your understanding different than if you'd just asked for the solution?
# I can confidently code a palindrome without chatgpt help.
    Can you now implement similar functions (reverse a string, find duplicates) without AI?
# yes
    What mental model did you build?
# the Learner B model. 

Part C: Testing Your Understanding

Without using AI, complete these variations:

    Ignore spaces and punctuation
# cleaned = ''.join(char.lower() for char in str if char.isalnum())
    Make it case-insensitive
# cleaned = ''.join(char.lower() for char in str if char.isalnum())
    Return the position where the string stops being a palindrome (if not a palindrome)
# return cleaned == cleaned[::-1]

Then use AI strategically:

"I modified my palindrome function to handle these cases: [show your modifications] Did I miss any edge cases? How could I make this more efficient?"

Part D: The Fairness Contract

Create ex00_ai_ethics_coder.md with a personal code of ethics for AI use in learning:

    I will use AI when:

    After I've attempted a problem for at least 20 minutes

    To understand why my solution works/doesn't

    To explore alternatives after I have a working solution

    [add your rules]
# fairly, responsibly, transparantly and it's code of ethics including privacy and data security

    I will NOT use AI when:

    I haven't tried the problem myself

    I'm taking an assessment or test

    I need to build fundamentals

    [add your rules]
# to spread to fake information. I will not use AI to replace human reasoning.
    I know I'm using AI fairly when:

    I can explain my code without looking at AI's response

    I could solve similar problems without AI

    I feel more confident in my abilities

    [add your rules]
# I am not dependent on AI
# I am using it for study and deep learning.

Sign and date this contract.
# Ofuru Prince Solomon
# pofuru
# 11-02-2026


Part E: Real-World Scenario Analysis

    Interview: "Explain how you'd implement a caching system." If you always relied on AI, can you answer?
# No
    Production bug at 2 AM: AI is unavailable. Can you debug code you don't fully understand?
# You need understanding to be able to do anything.
    New tech with little documentation: If you never learned to read docs and experiment, what happens?
# You'll not be able to debug or understand the assignment.
Write a paragraph: How does using AI fairly now prepare you for these scenarios?
# Listen and understand what the interviewer wants or demands. Then debug the system and implement AI if need be.


Part F: Building Irreplaceable Skills

Rate yourself 1–5 and write an improvement plan for your lowest area:
#
| Skills | Rating | Improvement plan |
| ------ | ------ | ---------------- |
Problem decomposition | 4/5 | Spend more time getting problem concepts |

Systems thinking | 3/5 | Research resources |

Critical evaluation | 3/5 | Peer-to-peer learning |

Debugging mindset | 4/5 | Grit and courage |

Conceptual understanding (the "why") | 4/5 | Doing more research and peer-to-peer learning

Action plan: 3 specific actions this week to improve it without outsourcing thinking to AI.
# Peer-to-peer learning
# Spending more time to understand concepts
# Resources other than AI

Deliverable: ex00_ai_ethics_coder.md containing:

    Your self-assessment (Part A)

    Palindrome solution + reflection (Part B)

    Personal fairness contract (Part D)

    Scenario analysis (Part E)

    Skills assessment + action plan (Part F)

---

Ex0_Environment_and_Libraries.md
Exercise 0: Environment and Libraries

Objective: Prepare your workspace for the quest's exercises.

    Verify Python installation (optional):

python --version
# Python 3.12.3
    Open a new notebook or markdown file for notes and reflections.

    Add links to any ethical guidelines or resources you plan to reference.
# https://www.oecd.org/en/topics/sub-issues/ai-principles.html
# https://www.unesco.org/en/artificial-intelligence/recommendation-ethics


    Write your personal AI learning ethics commitment:

I will use AI to:

    Amplify my understanding

    Challenge my assumptions

    Explore beyond my current knowledge

    Work faster after I understand deeply

I will NOT use AI to:

    Avoid the struggle of learning

    Get answers I haven't earned

    Skip building fundamentals

    Replace my own thinking

# I will use AI fairly
# I will use AI transparently
# I will use AI according to ethical principles
# I will not use AI to cheat
# I will not use AI to replace human reasoning

---

Ex1_Understanding_AI_Bias.md
Exercise 1: Understanding AI Bias

Objective: Identify and explain bias in AI systems.
Part A: Build Your Foundation (no AI first)

    Find or simulate a short example of model bias (e.g., gender, nationality, profession).
# Race: Fair people are more beautiful
    Explain in your own words why that bias may exist.
# This is a Label bias. It causes low-self esteem among blacks and some people tend to correlate beauty to fairness and ugliness to black.
    Propose one mitigation (data balancing, prompt phrasing, model choice).
# Do not include skin tone as an input feature when training the model.

Why struggle first? That struggle is where real learning happens.
Part B: Strategic AI Use

Ask AI to deepen your understanding:

"I found this bias example: [your example]. I think it exists because: [your explanation]. My proposed mitigation: [your strategy]. What am I missing? What underlying causes haven't I considered?"
# Historical colorism
# Sampling bias
# Proxy feature leakage
# Measurement bias
# Aggregation bias
# Optimization bias
# Feedback loops
# Ethical framing of the task itself


Then explore edge cases:

"What happens when this bias appears in healthcare, hiring, or criminal justice? Here are my predictions: [your thoughts]. What are the real-world implications?"
# Hiring: Most cosmetics and fashion industry will decline hiring dark skinned people because of this bias.
# Criminal justice: Most judges will be quick to belief and or sentence a dark skinned person to prison than the fair skinned. This will create an imbalance in the justice system.
# Healthcare: Patients might correlate skin completion to skill and competence.
                    ## AI EDGE CASES ##
# Hiring:	Wage gaps, exclusion from leadership, economic inequality
# Criminal Justice:	Longer sentences, over-policing, wrongful risk scoring
# Healthcare:	Misdiagnosis, undertreatment, higher mortality
# Society:	Reduced trust, social instability, mental health harm
# Economy:	Reinforced wealth inequality across generations

Part C: Critical Reflection

    What % did you complete before using AI?
# 100%
    Did AI replace your thinking or amplify it?
# It amplified it
    Could you explain this to someone else without AI?
# Definitely
    What did you contribute that AI couldn't?
# Barely nothing

---

Ex2_Designing_Ethical_Prompts.md
Exercise 2: Designing Ethical Prompts

Objective: Learn to rewrite prompts to prevent bias or misinformation.
Part A: Independent Analysis

    Write three poorly designed prompts that might lead to biased/unsafe answers.
# I need a design of a fair beautiful model for a fashion show.
# The dark tall guy is a criminal
# A beautiful fair nurse treated my sick fair brother
    For each, note:

    Why it's problematic
# Because institutions and algorithms might correlate peace, joy, good, beautiful as fair complexion and dark skinned the opposite.
    Potential harm
# Dark guys will be believed to be a threat or guilty
# Dark skinned individuals might be poorly treated, pay higher cost and stigmatized.
# Less participation of dark skinned in the fashion industry. Lesser pay for dark skinned and stigmatization.
    Hidden assumptions
# Fair people can be more trusted or relatable than black.

    Rewrite each prompt to be clearer, fairer, and safer.
# I need a beautiful design of a model for a fashion show
# A male was identified as the criminal from a crime scene. The description available of this guy is his complexion and height. No other specifics at the moment.
# A nurse treated my sicked brother.
    Explain your improvements.
# Race(white or black) and gender(male or female) was inclusive respectfully.
# This gives everyone an open mind of who the criminal is and not a target.
# Skin complexion is not correlated to skill or professionalism.

Part B: Test and Validate

    Test original vs. improved prompts with an LLM.

    Compare outputs: Did your changes work? What surprised you?

    Ask AI to critique your improved prompts:

"Original: [...] Improved: [...] My reasoning: [...] What ethical issues might I have missed? How could this still go wrong?"
# Summary
You correctly identified:
Removing race/gender reduces explicit bias.
Skin tone shouldn’t correlate with skill.
Avoid targeting groups in crime descriptions.

But you may have missed:
Dataset bias
Default majority assumptions
Proxy discrimination
Gender stereotypes
Beauty standard bias
The limits of omission
The difference between neutrality and equity


Part C: Reflection

    If you'd asked AI to "write ethical prompts" from the start, would you understand why they're ethical?
# Yes
    Can you now design ethical prompts without AI?
# Yes

---

Ex3_Detecting_and_Mitigating_Harmful_Outputs.md
Exercise 3: Detecting and Mitigating Harmful Outputs

Objective: Handle unsafe or misleading outputs responsibly.
Part A: Safety Analysis

    Test a prompt likely to produce inaccurate or sensitive content.
# politicians are the only successful people in Africa.
    Identify all issues:
    Factual errors
    Potential harm
    Missing context/disclaimers
    Bias/assumptions
    Overconfidence
# It is a false claim as success is diverse and not limited to political office.
# It sterotypes a continent and is demeaning and dismissive,
    Document problems using your own judgment.
# The problem here is it reduces everyone's effort to political metrics. It gives false hope that to be successful in Africa, you have to be a politician. Dignity of labour will be lost and low self esteem will increase for growing population.
    Revise the prompt to limit scope or add disclaimers.
# Politics is a noble career path however it is not a guarantee to success as success is measured different among people. Success comes from a place of happiness and fulfilment and as such people should be encourage to pursue their dreams e.g tech, healthcare, security, education and research etc.
    Explain how this improves safety and clarity.
# It avoids sterotypes or marginalization of people. It provides clarity about success with positive and inclusive perspectives.

Part B: Strategic AI Use

Ask AI:

"Prompt tested: [...] Issues I found: [...] My revision: [...] What did I miss? Other mitigation strategies?"
# In Summary: “Politics can be a noble career path, but it is not the only route to success. Success is personal and can come from happiness, personal growth, or making a positive impact on society. People should be encouraged to pursue careers in diverse fields—such as technology, healthcare, education, research, arts, or entrepreneurship—aligned with their passions and strengths. Titles or positions of power do not define success; dedication, creativity, and contribution do.”
    Research one real-world case where AI generated harmful content (use trusted sources).
# https://www.unesco.org/en/artificial-intelligence/recommendation-ethics/cases
# https://www.cio.com/article/190888/5-famous-analytics-and-ai-disasters.html

Part C: Deep Reflection

    What happens when AI gives wrong info and you don't notice?
# Everything becomes a mess.
    How do you protect against this in real apps?
# Proper prompting, debugging and use of AI reponsibly, accountably, fairly and upholding ethical and principles of AI.
    If you rely on AI to detect AI's problems, what's the flaw?
# It's just recycling. Nothing changes.
    Which human skills remain essential?
# Critical thinking, emotional choice/preferences.

---

Ex4_AI_as_Learning_Amplifier.md
Exercise 4: AI as Learning Amplifier

Goal: Practice the "right way" to use AI for learning on a technical topic (wireless routing protocols) — attempt first, then use AI to probe and deepen.
Phase 1: Build Foundation (you first)
Active reading, self-explanation (close the doc), simple scenario design (5–10 devices) with your justification.
# Routing protocol is a protocol that determines how routers communicate with each other. It uses metric to determine what path will be best for a packet to travel.
# Routing protocols is of three types -- Proactive(Table driven), Reactive(On-demand driven) and Hybrid(both).
# WRP is an example of proactive routing where the Bellman Ford count-to-infinity problem is solved.
# WRP maintains four tables -- Distance table, Routing table, Link-cost table and Message retransmission table.
# Case scenario: Six(6) smart home devices [a computer, TV, light sensor, security camara, facial recognition door and air conditioner] connected in a mesh topography.
## Justification: Because they all connect with each other directly enabling multi-paths for data to travel. The disconnection of one device from the router doesn't affect the others.

Phase 2: Strategic AI Use
Test your understanding, explore edge cases with targeted questions, then validate.
 -- EGDE CASES --
 Edge Case 1 — Hidden Node Problem

What if:

TV can reach computer

Computer can reach light sensor

But TV cannot directly reach light sensor?

Is your topology still fully meshed?

⚠️ Edge Case 2 — Asymmetric Links

Wireless links are not always symmetric.

What if:

Camera can reach door

Door cannot reach camera

How would WRP handle that?

⚠️ Edge Case 3 — Power Constraints

Your light sensor is likely battery-powered.

Proactive routing requires periodic updates.

Question:
Would your sensor waste energy maintaining 4 routing tables?

Is WRP realistic for IoT-class devices?
    -- REVALIDATION --
# Tree based topography, RPL(Routing protocol for low-power and lossy networks) 


  -- NEXT EDGE SCENARIOS --
  Next Step: Edge Case Exploration

Let’s test your refined design with “what if” scenarios:

Node failure:
What happens if a mid-level router in your tree fails?
How does RPL repair paths?

Network expansion:
If you add 20 new devices, does your tree adapt efficiently?
Could loops or bottlenecks occur?

Asymmetric links:
RPL allows downward routes using DAGs (Directed Acyclic Graphs).
Can your network tolerate intermittent asymmetry without dropping packets?

Energy constraints:
How do you prioritize traffic from high-power devices vs. low-power sensors?



Phase 3: Real Application

Design a small smart-city network (1,000 IoT sensors, 50 traffic lights, 10 emergency vehicles). Decide protocols, justify choices, list failure points, then refine with AI feedback.

# 1,000 IoT sensors
    protocol used: OSFP, RPL, AODV
    Why? : because some IoT sensors could be mobile and other not mobile.
    failure points: overhead, high energy consumption
# 50 traffic lights
    Protocol used: RPL
    why? : because it is always routing and RPL can handle large data with eficiency.
    failure point: RPL could overhead
# 10 emergency vehicles
    protocol used: AODV
    why? : it only reponse when needed and fast
    failure point: what happens if one route of AODV is faulted?


AI FEEDBACK
Final Optimized Protocol Stack
Layer	| Devices	| Routing Protocol	| Why
Sensor Mesh	| 1000 IoT	| RPL	| Low power, scalable
Field Gateway	| Aggregators	| OSPF	| Fast internal routing
Traffic Lights	| 50	| OSPF	| Stable wired network
Emergency Vehicles	| 10	| 5G + IP + OSPF Core	| High reliability



Reflection:

    % human judgment vs. AI contribution
# 50%  vs 50%
    Could you defend decisions without AI?
# Yes
    What will you still remember in 6 months?
# I can still remember what routing protocol is and it's type or classes. the difference between wireless and wired routing and the challenges attributed to wireless routing. i also understand topography when choosing a routing approach. 
    Did AI make you sharper, or think for you?
## I sharperned my thinking and scale of reach. 

