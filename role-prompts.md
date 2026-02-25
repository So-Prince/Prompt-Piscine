Ex0_Environment_and_Librarie.md
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

Ex1_Simulating_multiple_role.md
Objective: Understand how roles affect the model’s perspective.

    Write a prompt asking the same question (e.g., "What is climate change?").
# what is environmental degradation?
    Environmental degradation is the deterioration of the natural environment due to human activities and natural processes, resulting in damage to ecosystems, loss of biodiversity, and reduced quality of air, water, and soil.


    Add role instructions for at least 3 personas, such as:
        Scientist → technical explanation
# As a scientist, what is environmental degradation?
    A persistent reduction in ecosystem integrity characterized by loss of biodiversity, diminished ecosystem functions, altered biogeochemical cycles, and decreased environmental quality (air, water, and soil).

        Journalist → informative for the public
# As a journalist, what is environmental degradtion?
    Environmental degradation happens when the land, air, and water are harmed faster than they can recover. It’s not just an environmental issue — it’s a public health issue, an economic issue, and increasingly, a political issue.

        Critic → skeptical tone
# As a political critic, what is environmental degradation?
    The systematic erosion of natural systems driven by policy decisions, economic ideology, and institutional neglect.

    Compare how the answers differ.
# As the role changes, the tone, style and model of definition for the same instruction(question) changes. Each problem is seen with different lenses indicating significantly the importance of role attachment when prompting. For the scientist, he answers what is happening biologically and physically. For the journalist, he answers why people should care. While the political critic answers who's fault it is and why the system allows it.

---

Ex2_Role-based_mentoring_and_feedback.md
Objective: Use role-based prompts for personalized feedback.

    Ask the model to act as a coding mentor.

    Provide a simple piece of code (e.g., a Python function with a bug).
# Bugged python code
    def calculate_average(numbers):
    total = 0
    for i in range(len(numbers)):
        total += i
    return total / len(numbers)


scores = [80, 90, 100]
print("Average:", calculate_average(scores))



    Prompt the model: "Act as a mentor reviewing this code. Provide corrections and explain improvements."
# Debugged python code
     CORRECT CODE
def calculate_average(numbers):
    total = 0
    for number in numbers:
        total += number
    return total / len(numbers)

scores = [80, 90, 100]
print("Average:", calculate_average(scores))


    # ALTERNATIVE CODE
def calculate_average(numbers):
    if not numbers:
        return 0  # or raise ValueError("List cannot be empty")
    return sum(numbers) / len(numbers)

    # EDGE CASE: IF NOT NUMERIC VALUE
def calculate_average(numbers):
    numeric_values = [x for x in numbers if isinstance(x, (int, float))]
    if not numeric_values:
        return 0    # checks for non-numerical values like alphabets
    return sum(numeric_values) / len(numeric_values)


    Review the response and check if the role influences feedback style.
# It does. it reviews my bugged code, outlines the error and gives a step-by-step approach to debugging the issue. It also suggested possible edge cases and challenged me to it before providing solutions.

---

Ex3_Tone_variation_with_the_same_task.md
Objective: Control tone and style with explicit instructions.

    Choose one task (e.g., "Write an email inviting a candidate to an interview").
# Write for me a linkedin story for passing  my final BSc exams.
    Write two prompts:

        One for a friendly tone
# Write for me a linkedin story for passing my final BSc exams. Use a friendly tone
    I’m thrilled to share that I’ve officially passed my final BSc exams! It’s been a journey filled with late nights, endless coffee, and a lot of “just one more revision” moments.
    I want to take a moment to thank my incredible family, friends, and professors who supported me throughout this journey. Your encouragement kept me going, especially during the toughest weeks.
    This marks the end of one chapter and the start of an exciting new one. I’m looking forward to applying everything I’ve learned, continuing to grow, and exploring opportunities ahead.
    To anyone currently facing exams or big challenges: keep going! The hard work pays off. 🌟
    #Graduation #Milestone #NewBeginnings #BSc

        One for a professional tone
# Write for me a linkedin story for passing my final BSc exams. Use a professional tone
    I am pleased to announce that I have successfully passed my final BSc exams. This achievement represents the culmination of years of dedicated study, perseverance, and continuous learning.
    I am grateful for the guidance and support of my professors, mentors, and peers throughout this journey. Their insights and encouragement have been invaluable.
    As I close this chapter, I am eager to leverage the knowledge and skills I have acquired to contribute meaningfully in my professional endeavors and continue growing in my chosen field.
    #Graduation #ProfessionalGrowth #BSc #Achievement


    Compare the outputs and note how the tone changes while the content stays consistent.
# The tone is more chatty and informal when it's friendly when compared with a professional tone. The professional tone passes the message in a formal and concise manner.
