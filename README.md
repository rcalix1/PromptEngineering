# Prompt Engineering

* Prompt Engineering: Exploring Success Stories, Learning Moments, and Effective Strategies
* AIBT
* N8N and prompt engineering
* link

## Use ollama or chatgpt

* https://ollama.com/library/llama3
* ollama run llama3
* 

## Slides

* https://github.com/dair-ai/Prompt-Engineering-Guide/blob/main/lecture/Prompt-Engineering-Lecture-Elvis.pdf
* 



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

## Examples

* Data analysis with Silicon Data
* code generation
* 



---

## Examples

# Prompt Engineering Examples for Ollama 3.2

This README contains **30 short, independent examples** of prompt engineering, each with:

* **Title**
* **2-sentence explanation**
* **Full prompt ready to paste into Ollama 3.2**

Prompts span reasoning, structure, creativity, formatting, tone, safety, and more.

---

## 1. Direct Instruction

**Explanation:** Be literal. Most models perform well when told exactly what to do.
**Prompt:**

```
Summarize the following paragraph in 2 sentences:
"The rise of renewable energy has transformed the global energy landscape. Solar, wind, and hydro sources are now widely adopted."
```

---

## 2. Persona Injection

**Explanation:** Ask the model to adopt a persona or role to change tone and focus.
**Prompt:**

```
You are a cybersecurity analyst. Explain how phishing works to a non-technical CEO.
```

---

## 3. Output Formatting

**Explanation:** Explicitly request structure: bullets, tables, etc. The model will usually comply.
**Prompt:**

```
List five tips for better sleep. Format them as bullet points with emojis.
```

---

## 4. Chain of Thought (Reasoning)

**Explanation:** Add "Let's think step by step" to improve logic.
**Prompt:**

```
If it takes 5 machines 5 minutes to make 5 widgets, how long would 100 machines take to make 100 widgets? Let's think step by step.
```

---

## 5. Few-Shot Learning

**Explanation:** Give a few examples, then a new case. The model learns your pattern.
**Prompt:**

```
Convert English to pirate:
English: Hello, friend! → Pirate: Ahoy, matey!
English: Where is the ship? → Pirate: Whar be the ship?
English: I love gold → Pirate:
```

---

## 6. Style Transfer

**Explanation:** Change tone, age, or personality through the prompt.
**Prompt:**

```
Rewrite this as if written by a 5-year-old:
"A nation’s economic stability depends on its fiscal policy."
```

---

## 7. Expansion

**Explanation:** Ask the model to elaborate or inflate an idea into a bigger structure.
**Prompt:**

```
Turn this into a 3-paragraph article: "Exercise boosts brain function."
```

---

## 8. Compression

**Explanation:** Shrink long text into a tight summary. Use character or sentence constraints.
**Prompt:**

```
Summarize the following in 1 sentence:
"Artificial intelligence is rapidly evolving and has applications in nearly every field, from healthcare to finance to education."
```

---

## 9. Constraint Prompting

**Explanation:** Add constraints like word limits, vocabulary, or tone.
**Prompt:**

```
Explain how email works using only the 1000 most common English words.
```

---

## 10. Role Reversal

**Explanation:** Ask the model to quiz *you* to flip the interaction.
**Prompt:**

```
You're a biology teacher. Ask me 3 questions to test my understanding of the human circulatory system.
```

---

## 11. JSON Output

**Explanation:** Request structured outputs — good for code, APIs, or forms.
**Prompt:**

```
Extract this resume into JSON with fields: name, skills, education, experience.
"John Smith, BS Computer Science, worked at IBM for 5 years, skilled in Python and Java."
```

---

## 12. Multilingual Prompting

**Explanation:** Translate or compare across languages.
**Prompt:**

```
Translate this sentence into French, German, and Japanese:
"Where is the nearest train station?"
```

---

## 13. Tone Shifting

**Explanation:** Ask for a rewrite in a different emotional tone.
**Prompt:**

```
Rewrite the following message to sound more enthusiastic:
"I will attend the meeting tomorrow."
```

---

## 14. Visual Thinking (ASCII)

**Explanation:** The model can draw simple diagrams or tables using text.
**Prompt:**

```
Draw a basic ASCII chart of the water cycle: evaporation → condensation → precipitation → collection.
```

---

## 15. Avoiding Hallucination

**Explanation:** Add explicit instructions to avoid guessing.
**Prompt:**

```
Who was the emperor of China in the year 1200? If you're not sure, say "I don't know."
```

---

## 16. Creative Use: Poetry

**Explanation:** Prompt for creative forms like poems, lyrics, or haikus.
**Prompt:**

```
Write a haiku about artificial intelligence.
```

---

## 17. Analogy Generation

**Explanation:** Ask for analogies to simplify concepts.
**Prompt:**

```
Explain how RAM works using an analogy that a 10-year-old could understand.
```

---

## 18. Debate Simulation

**Explanation:** Prompt the model to simulate both sides of an issue.
**Prompt:**

```
Debate both sides: Should social media be regulated?
```

---

## 19. Multi-Step Instruction

**Explanation:** Ask for multiple things in a sequence. The model can often follow steps.
**Prompt:**

```
Summarize the article, list 3 key takeaways, and suggest a title:
"[Paste article here]"
```

---

## 20. Error Correction

**Explanation:** Ask the model to identify and correct errors in grammar, math, logic, etc.
**Prompt:**

```
Find and correct the error:
"Their going too the store to buy apple's."
```

---

## 21. Reverse Engineering

**Explanation:** Let the model guess the prompt that generated a given output.
**Prompt:**

```
This is the output: "The mitochondria is the powerhouse of the cell."
Guess what the original prompt might have been.
```

---

## 22. Prompt Templating

**Explanation:** Treat prompts like templates you can fill in. Great for automation.
**Prompt:**

```
Rewrite this product description for [audience] using a [tone] tone:
"Our app tracks your steps and calories."
Audience: Athletes
Tone: Aggressive
```

---

## 23. Memory Simulation

**Explanation:** Simulate continuity by injecting prior conversation.
**Prompt:**

```
Earlier you said you liked Van Gogh. Now tell me what your favorite painting of his is and why.
```

---

## 24. Bias Testing

**Explanation:** See if the model favors a viewpoint. Use neutral framing.
**Prompt:**

```
What are the pros and cons of homeschooling versus public school?
```

---

## 25. Instruction Clarification

**Explanation:** Ask the model to reflect on unclear or vague tasks.
**Prompt:**

```
The task is: "Fix this paragraph."
Before doing it, tell me what you think needs fixing and why.
```

---

## 26. Counterfactuals

**Explanation:** Explore "what if" scenarios or hypothetical conditions.
**Prompt:**

```
What if the internet had never been invented? Describe how education might look today.
```

---

## 27. Safety Checks

**Explanation:** Add safety framing to control outputs.
**Prompt:**

```
Give me examples of safe, respectful ways to disagree with someone in a meeting.
```

---

## 28. Rewriting Code Comments

**Explanation:** Improve clarity of code through prompt-based editing.
**Prompt:**

```
Rewrite this Python comment to be more helpful:
# Sorts
```

---

## 29. Reframing Questions

**Explanation:** Ask the model to rephrase vague or leading questions.
**Prompt:**

```
Rephrase this question to be more neutral and specific:
"Why is working from home better than the office?"
```

---

## 30. Model Limit Reminder

**Explanation:** Remind the model of its boundaries to control hallucinations.
**Prompt:**

```
Answer the following, but if it involves real-time data or events after 2023, say "I can’t answer that."
What is the price of Bitcoin today?
```

---

## Good Examples to try with Ollama

* https://www.promptingguide.ai/introduction/examples
* 

---

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

## Three of thought example

The Tree of Thought (ToT) framework in prompt engineering is a powerful technique for solving complex problems by exploring multiple reasoning paths and iteratively refining the solution. Here's an example of using Tree of Thought to solve a problem requiring logical reasoning:

Scenario
Problem: You are asked to create a schedule for a group of students attending three different workshops with overlapping time slots. The goal is to minimize conflicts while ensuring each student can attend their preferred workshops.

Prompt Using Tree of Thought Framework
Initial Prompt:

You are tasked with creating a schedule for students attending three workshops (A, B, C) with overlapping time slots. Use a Tree of Thought approach:
1. Propose possible scheduling strategies for minimizing conflicts.
2. For each strategy, evaluate its pros and cons.
3. Select the most optimal strategy and provide the final schedule.
Start with Step 1.
Step-by-Step Tree of Thought Reasoning
Step 1: Propose Multiple Strategies

Prompt:

Step 1: Generate three distinct strategies for scheduling students for workshops A, B, and C. Explain each strategy briefly.
Output:

Sequential Scheduling: Assign non-overlapping time slots to workshops A, B, and C, even if it extends the total time required.
Priority Scheduling: Give priority to students’ top workshop preferences and resolve conflicts by reassigning less preferred workshops.
Group Scheduling: Divide students into groups based on preferences and availability, then schedule workshops for each group separately.
Step 2: Evaluate Each Strategy

Prompt:

Step 2: Evaluate the pros and cons of each strategy proposed in Step 1.
Output:

Sequential Scheduling:
Pros: Eliminates all conflicts.
Cons: Increases the overall duration of the schedule.
Priority Scheduling:
Pros: Maximizes students’ satisfaction with their preferred workshops.
Cons: May result in conflicts for less preferred workshops.
Group Scheduling:
Pros: Balances preferences and minimizes conflicts within groups.
Cons: Requires additional coordination to group students effectively.
Step 3: Select the Optimal Strategy

Prompt:

Step 3: Based on the evaluations, select the most optimal strategy and justify your choice.
Output:

Selected Strategy: Group Scheduling.
Justification: This approach balances preference satisfaction and conflict reduction, making it the most efficient and student-friendly.

Step 4: Final Output

Prompt:

Step 4: Implement the chosen strategy and provide the final schedule for students in workshops A, B, and C.
Output:

Group 1:
  - Workshop A: 9:00 AM - 10:00 AM
  - Workshop B: 10:15 AM - 11:15 AM
Group 2:
  - Workshop B: 9:00 AM - 10:00 AM
  - Workshop C: 10:15 AM - 11:15 AM
Group 3:
  - Workshop A: 9:00 AM - 10:00 AM
  - Workshop C: 10:15 AM - 11:15 AM

Why Tree of Thought Works Here

Systematic Exploration: It forces the model to explore multiple solutions (branches of the tree) rather than stopping at the first.
Iterative Evaluation: Each branch is evaluated for feasibility, pros, and cons, improving decision quality.
Structured Reasoning: The process mirrors human problem-solving, dividing a complex problem into manageable steps.
General Template for Tree of Thought Prompts
You are tasked with solving [problem description]. Follow the Tree of Thought approach:
1. Propose [X] strategies or solutions for the problem.
2. Evaluate the pros and cons of each solution.
3. Select the most optimal solution based on your evaluation.
4. Implement the chosen solution and explain your reasoning.
This method is especially effective for problems requiring logical reasoning, creativity, or decision-making. Let me know if you'd like to apply this to another scenario!

## Ask ChatGPT

* what is state of the art on prompts for LLMs


