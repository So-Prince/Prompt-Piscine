Ex_0_Environment_and_Libraries.md
Objective: Set up the environment for Python development.

    Install Python (latest stable version, preferably 3.9+).

    Verify installation by running:
    python --version

# python3 --version

    Write and execute a Hello, World! program.
# print("Hello, World!")
    or
# word = "Hello, World!"
## print(word)

---

Ex_1_Logic_puzzle_with_explanation.md
Objective: Guide the model to solve a problem with explicit reasoning.

    Write a logic puzzle (e.g., "Alice is older than Bob, Bob is older than Carol. Who is the youngest?").
# Prince has 7 balls. He buys 2 more cans of balls. Each can has 3 balls. He gave 2 balls to Solomon. How many balls does he have now?
        Prince now has 11 balls.

    Prompt the model: "Explain your reasoning before giving the final answer."
# Prince has 7 balls. He buys 2 more cans of balls. Each can has 3 balls. He gave 2 balls to Solomon. How many balls does he have now? Explain your reasoning before giving the final answer.
        Let’s break it down step by step:

        Prince starts with 7 balls.

        He buys 2 cans, and each can has 3 balls:
        2×3=6 balls

        Now he has:
        7+6=13 balls

        He gives 2 balls to Solomon:
        13−2=11

        Final Answer: Prince now has 11 balls.

    Verify that the model provides step-by-step reasoning followed by the correct answer.
# The model gave a step-by-step reasoning followed by the correct answer after asking it to explain its reasoning. The first step stated the number of ball Prince had(7). Then it multiplied the number of ball by the number of cans bought(2*3=6). It added the initial and final balls(7+6=13) and then subtracted the number of balls given away from our sum total available balls(13-2) which resulted to our answer(11).

---

Ex2_Step-by-step_reasoning_prompt.md
Objective: Use structured prompting to encourage reasoning.

    Choose a math or coding problem (e.g., "Calculate the factorial of 5").
# What is the factorial of 7
        The factorial of 7 (written as 7!) is:
             7! = 5040.

    Prompt the model: "Let's think step by step before answering."
# Let's think step by step before answering. calculate the factorial of 7
            Factorial means multiplying a number by all positive integers below it down to 1.

            7!=7×6×5×4×3×2×1
            7!=7×6×5×4×3×2×1

            Now multiply in order:

            7 × 6 = 42
            42 × 5 = 210
            210 × 4 = 840
            840 × 3 = 2520
            2520 × 2 = 5040
            5040 × 1 = 5040

            So,
            7!=5040
	​

    Compare outputs with and without the reasoning instruction.
# Without the reasoning instruction = direct answer
# With the reasoning instruction = detailed step by step approach to how we arrive on the answer.

---

Ex3_Multi-step_question_answering.md
Objective: Break complex questions into smaller steps.

    Select a multi-step question (e.g., "What is 25% of the sum of 40 and 60?").
# Emma earns $2000 and buys groceries at a mini-mart supermarket at the cost of $800. He then transport with a cost of $2. 20% discount was placed on his goods. How much is left on Emma and what's 25% of his balance left?

    Create a prompt that asks the model to:

        1. Restate the problem
# Emma earns $2000. He buys groceries that cost $800, but a 20% discount is applied to the groceries. He also spends $2 on transportation. We are asked to find:
            How much money Emma has left after these expenses.
            What is 25% of his remaining balance.


        2. Break it into smaller steps
# 1. Calculate the discount on groceries.
    2. Calculate the final cost of groceries after discount.
    3. Subtract the groceries and transportation from Emma's earnings to get the remaining balance.
    4. Calculate 25% of the remaining balance.


        3. Solve each step before giving the final answer
# Step 3.1: Discount on groceries
            Original groceries cost = $800
            Discount = 20% of $800 = 
            0.20×800=160
            0.20×800=160

# Step 3.2: Final cost of groceries
            Final cost = $800 − $160 = $640

# Step 3.3: Remaining balance after groceries and transportation
            Transportation = $2
            Total expenses = $640 + $2 = $642
            Remaining balance = $2000 − $642 = $1358

# Step 3.4: 25% of remaining balance
            25% of $1358 = 0.25×1358
            Let's calculate step by step:
            1358×0.25=339.5

# Step 4: Final Answer
            Money left with Emma: $1358
            25% of his remaining balance: $339.50


    Review the reasoning process and check the accuracy of the final solution.
# Reasoning process enables us to get a detailed and correct response as the language model tackles the problem step by step. This is better and improved.

