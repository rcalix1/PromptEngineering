# Prompt Engineering

## Great sources

* https://github.com/dair-ai/Prompt-Engineering-Guide/tree/main

## General Tips for Designing Prompts

* https://www.promptingguide.ai/introduction/tips

##  Ilya Sutskever 

* Here are them with examples:

1. Communicate clearly and precisely when writing prompts.

This tip emphasizes the importance of unambiguous language in prompts. Clarity reduces the chance of misinterpretation by the AI model.
Example: Unclear prompt: "Make it better." Clear prompt: "Revise the given text to improve grammar, clarity, and conciseness while maintaining the original meaning."

2. Be willing to iterate rapidly, sending many prompts to the model in quick succession.
This approach allows for quick refinement and improvement of results. It's about not being afraid to try multiple variations quickly.

Example: First attempt: "Write a poem about spring." Refinement: "Write a haiku about cherry blossoms in spring." Further refinement: "Write a haiku about cherry blossoms in spring, emphasizing their ephemeral nature."

3. Consider edge cases and unusual scenarios when designing prompts.
This tip encourages thinking beyond the typical use case to ensure robustness.
Example: Basic prompt: "Calculate the average of these numbers: 5, 10, 15." Edge case consideration: "Calculate the average of these numbers, handling any non-numeric inputs or empty sets: 5, 10, 15, apple, -20, []"

4. Test your prompts with imperfect, realistic user inputs.
This ensures your prompts can handle real-world scenarios where users might not provide perfect input.

Example: Ideal input: "Translate 'Hello, how are you?' to French." Realistic input: "tranlate to french: hello how r u"

5. Read and analyze model outputs carefully.
This involves critically examining whether the model's response aligns with the intended outcome.
Example: Prompt: "List 5 capital cities in Europe." Output analysis: Check if all listed cities are indeed capital cities and located in Europe.

6. Strip away assumptions and clearly communicate the full set of information needed for a task.

This tip emphasizes providing all necessary context and avoiding implicit assumptions.
Example: Assumption-laden prompt: "Convert the temperature." Clear, detailed prompt: "Convert 25 degrees Celsius to Fahrenheit. Use the formula: °F = (°C × 9/5) + 32. Round the result to two decimal places."

7. Think about the "theory of mind" of the model when writing prompts.
This involves considering how the AI might interpret instructions differently than a human would.

Example: Potential misinterpretation: "Draw a house." Clearer prompt: "Describe in words a simple drawing of a house, including details about its shape, windows, door, and roof."

8. Use version control and track experiments when working with prompts.
This tip suggests treating prompts like code, using tools to manage iterations and experiments.
Example: Version 1: "Summarize the text in 100 words." Version 2: "Summarize the text in 100 words, focusing on key events and main characters." Version 3: "Provide a 100-word summary of the text, highlighting the plot progression and character development."

9. Ask the model to identify unclear parts or ambiguities in your instructions.

This approach leverages the model's capabilities to improve your prompts.

Example: Prompt: "Explain quantum entanglement. Then, identify any parts of this instruction that could be made clearer or more specific."

10. Be precise without overcomplicating.
This balances the need for clarity with the importance of simplicity.
Example: Overcomplicated: "Utilizing your vast knowledge of culinary arts and nutritional science, construct a detailed, step-by-step methodology for the creation of a simple yet nutritious sandwich, taking into account dietary restrictions and flavor profiles." Precise and simple: "Provide a recipe for a healthy sandwich, including ingredients and preparation steps."


11. Consider the balance between typical cases and edge cases.

This tip reminds us to handle unusual scenarios without losing focus on the main use case.
Example: Balanced prompt: "Create a function to calculate the area of a circle. The function should handle positive real numbers for the radius and return 'Invalid input' for negative or non-numeric inputs."

12. Think about how prompts integrate into larger systems.

This involves considering broader context and system constraints.

Example: System-aware prompt: "Generate a product description in 50 words or less, optimized for mobile display, focusing on key features and benefits."

13. Don't rely solely on writing skills; prompt engineering requires a mix of clear communication and systematic thinking.
This tip highlights the multifaceted nature of prompt engineering, combining linguistic and logical skills.

Example: Systematic prompt: "1. Analyze the given text for sentiment (positive, negative, or neutral). 2. Identify the main topic. 3. List three key points. 4. Suggest a follow-up question based on the content."

14. When working with customers, help them understand the realities of user input.
This involves educating clients about real-world usage patterns and potential variations in user input.
Example: Customer education: "Let's consider how users might actually phrase their questions. Instead of 'What's the weather forecast?', they might type 'weather tmrw' or 'is it gonna rain'. How should our system handle these variations?"

15. Practice looking at data and model outputs extensively.

This tip encourages familiarizing yourself with how the model responds to different inputs through hands-on experience.
Example: Practice exercise: Analyze the outputs of the same prompt across different AI models or different versions of the same model, noting differences in style, content, and adherence to instructions.

## Other

n "Design Patterns for Generative AI," you will discover an array of powerful techniques to help you:





Extract explicit and implicit information from GPT-4, refining your prompts to maximize clarity and precision.



Master the art of analogy-based explanations, reframing, and perspective-shifting to enrich your understanding of complex concepts.



Explore the world of hypothetical scenarios, ethical dilemmas, and counterfactual thinking to challenge your preconceptions and ignite your imagination.



Develop proficiency in brainstorming, lateral thinking, and problem restatement to stimulate innovative ideas and uncover hidden solutions.



Delve into the intricacies of cross-disciplinary insights, comparative analysis, and role-playing to broaden your horizons and foster empathy.



Embrace the power of storytelling, narrative techniques, and creative constraints to captivate your audience and convey your message with impact.

Each design pattern is accompanied by a clear explanation, practical examples, and real-world applications, making it easy for you to start implementing these techniques with GPT-4 right away. With this indispensable resource at your fingertips, you will be well-equipped to push the boundaries of AI-assisted creativity, analysis, and problem-solving.

In this book, I will demonstrate how we can use GPT-4 to gain a better understanding of the following questions:

Let’s attempt to understand several challenging questions that I will share with you how I used GPT-4 to to gain a firmer understanding of the question.  We will cover the following questions:





Is sensory grounding necessary for general intelligence?



How can we better understand the continuum of signs described by C.S.Peirce in semiotics?



How does evolutionary thinking relate to Alexander’s Nature of Order, and how can we use these ideas to understand other cognitive theories?



Can we lay the map for concepts that are beyond human comprehension?

CHAPTERS





1. Pattern Language Overview



2. Creational Patterns



3. Transformational Patterns



4. Coherence Patterns



5. Explainability Patterns



6. Procedural Patterns



7. Composite Patterns



8. Corrective Patterns



9. Recombinational Patterns



10. Variational Patterns



11. Modularity Patterns



12. Katas and Mediations



APPENDIX 1 - 2ND ITERATION PATTERNS



APPENDIX 2 - CLAUDE PATTERNS



APPENDIX 3 - BARD PATTERNS


## more


### Example 1: Code Generation
Prompt:

Write a Python function to implement the bubble sort algorithm. Include comments explaining each step.
Breakdown:

Task Definition ("Write a Python function"):
Clearly specifies the task as writing code, which helps the model avoid confusion.
Algorithm Name ("bubble sort algorithm"):
Names the specific algorithm to implement, guiding the model toward the correct solution.
Instruction to Include Comments:
Adds a requirement for clarity and explanation, ensuring the generated code is understandable for learners or reviewers.
Why These Elements Matter:

Without specifying "bubble sort," the model might guess incorrectly and provide a different sorting algorithm.
Including "comments explaining each step" ensures the output is educational, useful for understanding, and well-documented.


### Example 2: Content Summarization
Prompt:

Summarize the following article in 100 words, highlighting the main points: [Paste text here].
Breakdown:

Action Verb ("Summarize"):
Tells the model what action to perform, narrowing the task to a summary.
Output Constraint ("in 100 words"):
Sets a clear boundary for the output length, ensuring concise results.
Focus Area ("highlighting the main points"):
Clarifies what aspects of the article are most important, avoiding irrelevant details.
Why These Elements Matter:

Without specifying "100 words," the model might create a summary that is too long or too short.
Adding "highlighting the main points" prevents the summary from being vague or missing key information.

### Example 3: Sentiment Analysis
Prompt:

Analyze the sentiment of the following review and classify it as Positive, Negative, or Neutral: "The product quality was excellent, but the delivery was delayed by two weeks."
Breakdown:

Task Definition ("Analyze the sentiment"):
Directs the model to focus on analyzing emotions or tone.
Classification Labels ("Positive, Negative, or Neutral"):
Provides predefined categories, helping the model structure its response.
Input Text Example:
Supplies concrete text for analysis, making the task actionable.
Why These Elements Matter:

Including specific labels ensures that the output aligns with the desired categories.
A concrete input example eliminates ambiguity and ensures the model works with a clear dataset.


### Example 4: Text Rewriting
Prompt:

Rewrite the following paragraph to make it suitable for a fifth-grade reading level: [Paste text here].
Breakdown:

Action Verb ("Rewrite"):
Focuses the task on transformation, not analysis or interpretation.
Target Audience ("fifth-grade reading level"):
Defines the level of complexity the model should aim for in the rewrite.
Why These Elements Matter:

Without specifying "fifth-grade reading level," the model might rewrite text for a different audience, making it less effective.
"Rewrite" ensures the task is generative rather than interpretive.


### Example 5: Idea Generation
Prompt:

Generate five unique marketing ideas for a sustainable clothing brand targeting young adults.
Breakdown:

Action Verb ("Generate"):
Instructs the model to create original content.
Number Constraint ("five unique ideas"):
Sets an exact expectation, ensuring the response is structured and complete.
Context ("sustainable clothing brand targeting young adults"):
Provides essential details about the audience and brand values, guiding the model's creativity.
Why These Elements Matter:

Without the "five unique ideas" constraint, the model might provide too few or duplicate suggestions.
Context like "sustainable" and "young adults" focuses the model on relevant themes and demographic considerations.


### Example 6: Educational Tutoring
Prompt:

Explain the concept of quantum entanglement in simple terms for a high school student.
Breakdown:

Specific Concept ("quantum entanglement"):
Narrows the scope to a particular topic, avoiding irrelevant explanations.
Audience Specification ("high school student"):
Guides the level of complexity, ensuring the explanation is accessible.
Why These Elements Matter:

Without specifying "high school student," the model might default to overly technical explanations.
Naming the concept ensures the output is focused and relevant.
General Best Practices for Prompt Engineering
Start with an Action Verb:
Clearly define the task (e.g., "Write," "Summarize," "Analyze," "Explain"). This minimizes ambiguity and sets the right expectation.
Provide Specific Context:
Add enough detail about the topic, audience, or constraints to guide the model effectively.
Set Clear Output Constraints:
Define word limits, number of items, or specific formats for the output. This ensures responses are concise, complete, and structured.
Use Examples or Templates:
Including examples clarifies expectations and helps the model align with the desired style or format.


