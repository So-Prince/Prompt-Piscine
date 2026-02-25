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

Ex1_Summarization_pattern.md
Objective: Create a reusable prompt for text summarization.

# My Text
        Griselda Blanco (born February 15, 1943, Santa Marta?, Colombia—died September 3, 2012, Medellín) was a Colombian cocaine trafficker who amassed a vast empire and was a central figure in the violent drug wars in Miami in the 1970s and ’80s.Although there is some confusion about her birth location, a number of sources give it as Santa Marta, Colombia, where Blanco was baptized. She grew up in poverty, and her life of crime reportedly began at an early age. According to some accounts, at age 11 she helped kidnap a boy, and, after his wealthy family refused to pay the ransom, she fatally shot him. She also was alleged to be a pickpocket and prostitute. While still a teenager, she married a small-time criminal, and the couple had three children. However, they subsequently divorced—Blanco was believed to have ordered his murder several years later—and in the early 1970s she began a relationship with Alberto Bravo, a drug trafficker whom she ultimately married. It was through him that she became involved in the cocaine trade. With New York City as their base, the couple began bringing the drug into the United States. Aided by Blanco’s creativity—she notably had lingerie made with secret compartments to smuggle drugs—the couple created an extensive and highly profitable operation. However, facing drug charges, Blanco returned to Colombia in 1975. That year she came to believe that her husband was stealing money, and a shoot-out between the couple resulted in Bravo’s death. Living up to her nickname as the “Black Widow,” she reportedly later had her third husband killed as well. By the late 1970s Blanco had moved to Miami, where she made her reputation as the “Godmother of Cocaine.” Seeking to eliminate her competition, she displayed a brazen ruthlessness that plunged the city into a period of violence that became known as the Cocaine Cowboy Wars. She allegedly ordered numerous murders, many of which were committed by gunmen on motorcycles, a practice she was said to have invented. In addition, a number of the killings occurred in broad daylight, including a shoot-out at a local mall in 1979. Backed by such violence and a sharp cunning, Blanco became one of the world’s wealthiest drug traffickers. According to reports, she smuggled more than three tons of cocaine into the United States annually, netting some $80 million per month. Blanco embraced her criminal persona, notably naming one of her sons Michael Corleone, after a crime boss in the Godfather series. She also enjoyed a lavish lifestyle that included luxury homes and hedonistic parties. Targeted by rivals and fearing for her life, Blanco moved to California in 1984. However, the following year she was arrested and taken to New York to face the 1975 drug charges. Found guilty in 1985, she received the maximum sentence of 15 years in prison, though she reportedly continued to run her empire while incarcerated. During this time, officials looked to press additional charges against Blanco, who was implicated in more than 200 murders. In 1994, after one of her hit men, Jorge Ayala, agreed to testify against her, Blanco was charged with three murders, including the fatal shooting of a former enforcer’s two-year-old son, who was killed during a failed attempt on his father’s life. Prosecutors were seeking the death penalty, but Ayala’s credibity was undermined when it was revealed that he had been having phone sex with secretaries in the prosecuting attorney’s office; one of the women claimed that she was acting on orders of the prosecutor, who denied the charges. In 1998 Blanco ultimately pled guilty in exchange for a reduced sentence, and six years later she was released and deported to Colombia. Blanco reportedly retired from a life of crime, but in 2012 she was killed by a gunman on a motorcycle as she left a butcher shop in Medellín.


    Write a weak prompt: "Summarize this text."
# Summarize this text
        Griselda Blanco (1943–2012) was a Colombian cocaine trafficker, infamous as the “Godmother of Cocaine” for her role in the violent Miami drug wars of the 1970s and ’80s. Born in Santa Marta, Colombia, she grew up in poverty and began a criminal life early, including kidnapping and murder. She married several men, allegedly having at least two killed, and became deeply involved in the cocaine trade through her second husband, Alberto Bravo. Blanco developed innovative smuggling methods and built a vast empire, reportedly importing over three tons of cocaine into the U.S. annually and earning $80 million per month. Known for her ruthlessness, she allegedly ordered hundreds of murders, often carried out in daylight by motorcycle gunmen. Arrested in 1985, she served 14 years in prison, continued her criminal operations while incarcerated, and was eventually deported to Colombia in 2004. Despite reportedly retiring, she was killed by a motorcycle gunman in Medellín in 2012.

Why weak?
    No length requirement
    No structure
    No focus
    No clarity about what to ignore
    Results will vary wildly


    Refine it into a reusable pattern:

        "Summarize the following text in 3 bullet points, focusing on the main arguments and ignoring examples."
# Summarize the following text in 3 bullet points, focusing on the main arguments and ignoring examples.
        -- Griselda Blanco rose from poverty in Colombia to become a major cocaine trafficker, building a highly profitable smuggling empire in the United States during the 1970s and 1980s.

        -- She played a central role in Miami’s violent drug wars, earning a reputation for extreme ruthlessness and allegedly ordering numerous murders while expanding her criminal network.

        -- Arrested in 1985 and later charged in multiple murder cases, she served prison time, was released and deported to Colombia in 2004, and was killed in 2012.

This is better because:
    Specifies format (bullet points)
    Specifies length (3)
    Specifies focus (main arguments)
    Specifies what to exclude (examples)



    Test it with at least two different inputs (e.g., a news article and a technical blog).

# NEWS ARTICLE
    Input: Summarize the news article[Mourinho and Benfica under fire after Real Madrid’s Vinicius alleges racism] in 3 bullet points, focusing on the main arguments and ignoring examples.

    Output: 
            -- Real Madrid’s Vinícius Júnior accused a Benfica player of using a racist slur during their Champions League match, leading to a stoppage of play under anti‑racism protocols and overshadowing Real’s 1‑0 win.
            -- Benfica manager José Mourinho drew criticism for his response, suggesting Vinícius’ celebration helped provoke the incident and defending the club against accusations of racism rather than clearly condemning racial abuse.
            -- The controversy prompted a backlash from pundits and others in football, with many condemning how the situation was handled and renewing broader concerns about racism in the sport.
# TECHNICAL BLOG
    Input: Summarize the technical blog[An AI Survival Guide for Curating Your Digital Inner Circle] in 3 bullet points, focusing on the main arguments and ignoring examples.

    Output: 
            -- It argues that to thrive in an AI‑driven world, individuals and organizations should carefully select and manage a small “inner circle” of specialized AI agents tailored to their specific needs rather than relying indiscriminately on many generic tools.
            -- The guide emphasizes that strategic curation of AI — choosing high‑value agents and aligning them with goals — enhances productivity and decision‑making more effectively than unfocused adoption of AI technologies.
            -- It suggests that this curated approach helps maintain human control, clarity, and relevance in digital workflows as AI becomes more pervasive across personal and business environments.

---

Ex2_Data_extraction_template.md
Objective: Extract structured data from unstructured input.

    Choose an unstructured text (e.g., "John Doe, age 29, lives in Paris and works as a software engineer.").
# John Doe, age 29, lives in Paris and works as a software engineer.

    Create a template prompt:

        "Extract the following fields from the text: Name, Age, Location, Occupation. Return the output in JSON format."
# Unstructured text: John Doe, age 29, lives in Paris and works as a software engineer.Extract the following fields from the text: Name, Age, Location, Occupation. If any field is missing in the text, use null. Return the output in JSON format.

    Validate the output and ensure consistency across multiple inputs.
# Output:
            {
            "Name": "John Doe",
            "Age": 29,
            "Location": "Paris",
            "Occupation": "software engineer"
            }

---

Ex3_Prompt_transformation_with_patterns.md
Objective: Strengthen weak prompts using patterns.

    Take a vague or under-specified prompt (e.g., "Write about climate change.").
# Write about climate change
            Climate change is one of the most pressing global challenges of our time. It refers to long-term shifts in temperature, weather patterns, and environmental conditions on Earth, largely driven by human activities such as burning fossil fuels, deforestation, and industrial processes. These activities release greenhouse gases—like carbon dioxide and methane—into the atmosphere, trapping heat and causing the planet’s average temperature to rise, a phenomenon commonly known as global warming.
            The impacts of climate change are widespread and severe. Rising temperatures contribute to more frequent and intense heatwaves, droughts, and wildfires. Melting glaciers and polar ice caps lead to rising sea levels, which threaten coastal communities. Ecosystems are also affected, with many species struggling to adapt to changing conditions, resulting in biodiversity loss. Agriculture, water resources, and human health are increasingly vulnerable to these environmental shifts.
            Addressing climate change requires coordinated global action. Transitioning to renewable energy sources, improving energy efficiency, protecting forests, and promoting sustainable agriculture are key strategies to reduce greenhouse gas emissions. Policies like the Paris Agreement aim to limit global warming to well below 2°C above pre-industrial levels. Individuals can also contribute by reducing their carbon footprint through lifestyle choices such as using public transport, conserving energy, and supporting sustainable products.
            Ultimately, climate change is both an environmental and social challenge. Combating it effectively requires collective action, innovation, and a commitment to building a more resilient and sustainable world.


    Transform it using instructional or comparative patterns:

        Instructional: "Write a 200-word explanation of climate change for high school learners."
# Write a 200-word explanation of climate change for high school learners.
            Climate change is the long-term change in Earth’s climate, especially a rise in global temperatures, caused mostly by human activities. When we burn fossil fuels like coal, oil, and gas for energy, or cut down forests, we release gases such as carbon dioxide and methane into the atmosphere. These are called greenhouse gases because they trap heat from the sun, making Earth warmer—a process known as the greenhouse effect.
            The effects of climate change are visible all over the world. Temperatures are rising, glaciers and ice caps are melting, and sea levels are increasing. This leads to more extreme weather events, like hurricanes, heatwaves, floods, and droughts. Plants and animals struggle to survive in changing conditions, which can cause some species to disappear. Humans are affected too, through damage to homes, crops, and health risks like heat stress and disease.
            Fighting climate change requires both global and personal action. Countries can reduce emissions by using renewable energy such as solar and wind power, protecting forests, and promoting cleaner transportation. Individuals can help by saving energy, recycling, planting trees, and making sustainable choices. Understanding climate change is important because the actions we take today will determine the future of our planet, the ecosystems, and the generations to come.

        Comparative: "Compare the effects of climate change on coastal vs inland regions in 5 bullet points."
# Compare the effects of climate change on coastal vs inland regions in 5 bullet points.
            -- Rising Sea Levels: Coastal regions face flooding and erosion due to melting glaciers and thermal expansion of oceans, while inland areas are less directly affected by sea-level rise.

            -- Storm Impact: Coastal areas experience stronger hurricanes, cyclones, and storm surges, causing property damage and displacement; inland regions may face severe windstorms and tornadoes, but less risk from ocean-based storms.

            -- Temperature Changes: Inland regions often see more extreme temperature fluctuations—hotter summers and colder winters—compared to coastal areas, where the ocean moderates temperatures.

            -- Water Availability: Inland regions may face droughts and reduced freshwater supplies as rivers dry up, whereas coastal areas can experience saltwater intrusion into freshwater aquifers.

            -- Ecosystem Stress: Coastal ecosystems like mangroves, coral reefs, and estuaries are highly vulnerable to warming oceans and acidification, while inland ecosystems, such as forests and grasslands, struggle with heat stress, wildfires, and shifting rainfall patterns.


    Document the improvement in clarity and usefulness of the outputs.
# Vague or under-specified prompts gives unclear and vast response. Instructional or comparative patterns prevents ambuigity and presents results to user demand.
