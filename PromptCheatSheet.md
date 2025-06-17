Prompting Cheat Sheet: Go From Basic Questions to Expert Results
Section 1: Prompting Fundamentals (The Core Recipe)
This section covers the absolute must-knows for writing any successful prompt.

The Golden Rule: Your output quality can never exceed your input quality. To get better answers, ask better questions.

Key Parameters: The AI's "Mood Ring"
Temperature: Controls randomness and creativity.

Low Temp (e.g., 0.2): For factual, focused, and predictable outputs.

Use for: Summaries, code generation, translations, factual Q&A.

High Temp (e.g., 0.8): For creative, surprising, or novel outputs.

Use for: Brainstorming, fiction writing, poetry, generating diverse ideas.

Essential Components of a Good Prompt
Assign a Role/Persona: Tell the AI who to be.

Example: "Act as a senior software engineer..."

Provide Clear Context: Give necessary background, but keep it brief.

Example: "I'm writing a blog post for beginners. Explain the concept of..."

Define the Output Format: State exactly how you want the answer structured.

Example: "Provide the answer as a JSON object with keys 'name' and 'role'."

Set Constraints: Give the AI clear boundaries.

Example: "Limit your response to 100 words and do not include personal opinions."

Structuring Your Prompt for Success
Use Delimiters: Employ separators like ###, ---, or XML tags (<example>) to clearly distinguish instructions from context.

Placement is Key: Put your most critical instructions at the very start or end of the prompt for maximum visibility.

Section 2: Key Prompting Techniques (The Power Tools)
Use this table to choose the right advanced technique for your specific task.

Technique

Core Purpose

Best For

Do Not Use For

Example

Few-Shot Prompting

Guiding the AI by showing it examples of the exact input/output format you want.

Tasks requiring a specific format, style, or nuanced judgment (like sentiment analysis).

Simple, straightforward tasks where a direct instruction is sufficient.

"Input: 'Great film!' -> Output: Positive. Now, analyze: 'It was a decent effort.'"

Chain-of-Thought (CoT)

Forcing the AI to "show its work" by breaking down its reasoning into sequential steps, improving accuracy.

Logic puzzles, math problems, and complex planning that requires reasoning.

Simple Q&A, creative tasks, or when response time is critical (as CoT is slower).

"Solve this logic puzzle. First, think step-by-step to deduce the solution, then state the final answer."

Least-to-Most Prompting

Solving a complex problem by breaking it into a sequence of easier, manageable sub-problems.

Multi-part problems where later steps depend on the solutions to earlier ones (e.g., building a story).

Simple, one-shot requests that don't have multiple dependent parts.

"First, describe a detective. Second, using that description, introduce the lost pet's owner..."

Self-Consistency

Improving accuracy by generating multiple reasoning paths and choosing the most frequent or logical answer.

High-stakes questions where accuracy is critical and you need a reliable, robust answer.

Creative or brainstorming tasks where variety is desired over a single "correct" answer.

"Provide three distinct perspectives on the pros and cons of remote work for employee well-being."

Self-Refinement

Instructing the AI to critique and improve its own generated response based on your criteria.

Polishing an output to meet high-quality standards without multiple manual re-prompts.

Quick, first-draft generation where speed is more important than a perfectly polished result.

"Review your previous answer for ambiguities, then revise it to be more concise and factual."

Knowledge Generation

Forcing the AI to state what it knows about a topic before answering to ground its response in facts.

Combating hallucinations and ensuring answers are based on specific, up-to-date knowledge.

Simple questions relying on common knowledge the AI already possesses.

"Before discussing its impact, summarize the current known theories on quantum entanglement."

Expert-Level Techniques (Use with Caution)
Note: The following techniques are highly specialized. They can be very powerful but are often more complex to implement, can be token-intensive (costly), and are best reserved for specific, challenging problems where other methods have fallen short. Master the basics first, as these methods require more effort and may not always yield better results for simple tasks.

Technique

Core Purpose

Best For

Do Not Use For

Example

Tree/Graph of Thought (ToT/GoT)

Allowing the AI to explore, evaluate, and navigate multiple branching reasoning paths at once.

Very complex problem-solving with many interdependent parts, strategic planning, or creative ideation with constraints.

Most standard tasks. This technique is computationally expensive and slow.

"Brainstorm solutions for urban traffic. Branch 1: Public transport. Branch 2: Infrastructure. Branch 3: Behavioral shifts. Evaluate and synthesize."

Directional Stimulus

Subtly guiding the AI's focus towards specific keywords, themes, or styles within the prompt.

Ensuring certain concepts are consistently included or a specific tone is maintained without rigid constraints.

Broad, open-ended exploration where you don't want to narrow the AI's focus.

"When describing a futuristic city, always incorporate themes of sustainability and community."

Automatic Prompt Engineering

Using an AI to generate or refine prompts for another AI to improve its performance on a specific task.

Optimizing prompts for a complex, repetitive task where you are unsure of the best phrasing.

Simple, one-off tasks where manually writing the prompt is faster and more efficient.

"Given the task 'Generate social media captions for a new coffee shop,' create 3 alternative prompts to get more creative results."

Section 3: Troubleshooting (The First-Aid Kit)
When your prompts go wrong, consult this quick-glance guide for the most common problems and their fixes.

Problem

Quick Fixes

The output is factually incorrect or "hallucinated."

1.  Lower the Temperature (e.g., to 0.2) to reduce creativity. 
 2. Provide grounding context within the prompt (e.g., "Using the article below..."). 
 3. Ask it to cite sources.

The AI is ignoring my instructions.

1.  Place instructions at the start or end of the prompt. 
 2. Use delimiters like ### INSTRUCTION ### to make them stand out. 
 3. Break the task into smaller, simpler steps.

The output is in the wrong format.

1.  Be explicitly clear about the format (e.g., "Format the output as a JSON object..."). 
 2. Provide a Few-Shot example showing the exact format.

The AI refuses to answer ("I can't do that").

1.  Your prompt may be triggering a safety filter. Rephrase it from a compliant, educational, or hypothetical perspective. 
 2. Do not use this to bypass legitimate safety protocols.

The output is too generic or repetitive.

1.  Increase the Temperature (e.g., to 0.7-0.8). 
 2. Be much more specific (e.g., ask for "a noir detective story set in a haunted laundromat"). 
 3. Add negative constraints (e.g., "Avoid using clichés").

Token usage or cost is too high.

1.  Make prompts more concise. Trim unnecessary words. 
 2. For large documents, have the AI summarize the text first, then prompt the summary.

When All Else Fails...

Restart the session. This is the AI equivalent of "turning it off and on again" and can resolve many unexpected issues.

