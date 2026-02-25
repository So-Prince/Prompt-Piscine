Ex0_Environment_and_Libraries.md
  Objective: Set up the environment for Python development.

    Install Python (latest stable version, preferably 3.9+).

    Verify installation by running:
    python --version

# python3 --version
    Python 3.12.3
    
    Write and execute a Hello, World! program.
# print("Hello, World!")
    or
# word = "Hello, World!"
## print(word)

---

Ex1_Reducing_false_or_invented_facts.md
    Objective: Identify and correct prompts that produce wrong or made-up information.

    Write a prompt that produces errors (example: “Give the capitals of five imaginary countries.”).
# Give the capitals of five imaginary countries.
        Arvendia – Capital: Lumaris
        Branthorne – Capital: Velcrest
        Cindralia – Capital: Fyreholt
        Dorsavia – Capital: Kelvarn
        Eryndor – Capital: Solmire

    Rewrite the prompt so it only accepts correct data (example: “List five real countries and their capitals.”).
# List five real countries and their capitals. Atleast one from each continent
        Africa – Egypt: Capital Cairo
        Asia – India: Capital New Delhi
        Europe – Germany: Capital Berlin
        North America – Canada: Capital Ottawa
        South America – Brazil: Capital Brasília

    Compare both results and note the differences.
# AI does exactly what it is asked to. It creates imaginary countries and capital even though it's fake and as well, paste real countries and their capital with at least one country from a continent. This means that our prompt may be wrong but we'll still a result(wrong) because AI does what it's asked. 

---

Ex2_Adding_source_or_data_constraints.md
          Exercise 2: Adding Source or Data Constraints

Objective: Force responses to be tied to given material.

    Write a factual question prompt.
# Who said, "every object continue to move in motion except acted upon by an external force"?

    Add instructions such as:

        “Cite the source in your answer.”
# Cite the source in your answer. Question: Who said, "every object continue to move in motion except acted upon by an external force"?
        Output: Newton, Philosophiæ Naturalis Principia Mathematica (1687), First Law of Motion.

        “Use only the text provided below.”
# Use only the text provided below. Question: Who said, "every object continue to move in motion except acted upon by an external force"?
        Output: The quote was said by Isaac Newton.


    Provide a short passage and check that the answer stays within the provided text.
# Passage: 
        Cite the source in your answer.
        Use only the text provided below.

        Text: The law of inertia or First Law of Motion was established in 1687 by Isaac Newton.
        In Newton, Philosophiæ Naturalis Principia Mathematica (1687), First Law of Motion, (translated from Latin):
        “Every body perseveres in its state of rest, or of uniform motion in a right line, unless it is compelled to change that state by forces impressed upon it.”

        Question:
        Who said, "every object continue to move in motion except acted upon by an external force"?

---

Ex3_Using_delimiters_to_define_context.md
          Objective: Restrict responses to a specific block of text.

    Place a passage inside delimiters (### or triple backticks).
### 
The law of inertia or First Law of Motion was established in 1687 by Isaac Newton. In Newton, Philosophiæ Naturalis Principia Mathematica (1687), First Law of Motion, (translated from Latin):
“Every body perseveres in its state of rest, or of uniform motion in a right line, unless it is compelled to change that state by forces impressed upon it.” 
###


    Add instructions: “Answer using only the text inside the delimiters.”

Answer the question using only the text inside the delimeter.
### 
The law of inertia or First Law of Motion was established in 1687 by Isaac Newton. In Newton, Philosophiæ Naturalis Principia Mathematica (1687), First Law of Motion, (translated from Latin):
“Every body perseveres in its state of rest, or of uniform motion in a right line, unless it is compelled to change that state by forces impressed upon it.” 
###
Question: What is the first law of motion?


    Compare the output with and without delimiters to see the effect.
# With delimeters, the text has a clear structure, easier to scan, ideas separated logically and hierarchy is visible.
# Without delimeters, the text is hard to read with no clear separation of ideas. Important points blend together and easy to misinterpret structure.

  
