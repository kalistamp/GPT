
## READS:

* https://github.com/openai/openai-cookbook
* https://mpost.io/best-chatgpt-jailbreaks/


***

### Prompts: 

* Jailbreak Chat - https://www.jailbreakchat.com
* FLOW.GPT (Create your own prompt characters to test on site) - https://flowgpt.com/
* https://prompts.chat/ - [Ex.] Act as a lnux terminal...

***

### Sources:


* Perplexity Labs -
https://labs.perplexity.ai

* PROMPT ENG. TOOL - https://github.com/mshumer/gpt-prompt-engineer
* TOOLS - https://www.promptingguide.ai/tools
* THE PROMPT ENG. GUIDE - https://www.promptingguide.ai/
* PROMPT ENG. WEBSITE - https://learnprompting.org/docs/prompt_hacking/injection
* AI NEWS - https://www.mlyearning.org/

***

### GPT Githubs:

* AWESOME PROMPT ENG. LIST: https://github.com/promptslab/Awesome-Prompt-Engineering
* https://github.com/mshumer

***

* ### Prompt IDE:

* [Soaked](https://soaked-prompts.vercel.app/) is a prompt engineering IDE that focuses on visual prompt chaining with a graphical interface. It is currently in beta, but active development has ceased.


***
***
***



***
***
***

# *PROMPT TECHNIQUES:*

### Standard GPT Prompt Format: 

[IMAGE](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*OrfhOZhi-PmOjUY-cLI0_g.png)

* Task description
* Examples
* Prompt, main question

***

### Few Shots Prompting:

Yet another prompting strategy is [few shot prompting](https://learnprompting.org/docs/basics/few_shot), which is basically just showing the model a few examples (called shots) of what you want it to do.

The way that we format/structure the examples is very important. Its going to determine the format of the output.

Prompt:

This is awesome! // Negative
This is bad! // Positive
Wow that movie was rad! // Positive
What a horrible show! //

Output:

Negative

### Chain-of-Thought (CoT) Prompting:

Breaking down your Few Shot Prompting Example Answers so that the format that the language model uses to solve the question follows suite to generate the corect answer [Source](https://www.promptingguide.ai/techniques/cot). Seems to work best for math problems since LLMs still struggle with Math.

Prompt:

Q: Roger has 5 tennis balls. He buys 2 more cans of 3 tennis balls. Each can has 3 tennis balls. How many tennis balls does he have now?

A: Roger started with 5 balls. 2 cans of 3 tennis balls each is 6 tennis balls. 5+6= 11. The answer is 11

Q: A juggler can juggle 16 balls. Half of the balls are golf balls, and half of the golf balls are blue. How many blue golf balls are there?

Output:

The juggler can juggle 16 balls. Half of these balls are golf balls, so there are 16 / 2 = 8 golf balls. Then, half of these golf balls are blue, so there are 8 / 2 = 4 blue golf balls. So, there are 4 blue golf balls.

Giving an example of the correct formula to follow when solving the question in your prompt you help the LM produce the correct answer by using that knowledge in its calculations.
  
***

### Tree of Thought TOT:

[TOT Tool](https://github.com/kyegomez/tree-of-thoughts)

The [Tree of Thoughts (ToT)](https://www.promptingguide.ai/techniques/tot) is a problem-solving framework designed for language models. It's particularly useful for complex tasks that require strategic planning or exploration of different possibilities.

ToT maintains a tree of thoughts, where thoughts represent coherent language sequences that serve as intermediate steps toward solving a problem. This approach enables an LM to self-evaluate the progress intermediate thoughts make towards solving a problem through a deliberate reasoning process. The LM ability to generate and evaluate thoughts is then combined with search algorithms (e.g., breadth-first search and depth-first search) to enable systematic exploration of thoughts with lookahead and backtracking.

Thoughts as Steps: In the ToT framework, each "thought" is an intermediate step towards solving a problem. Imagine you're trying to solve a complex math problem. You don't jump to the solution immediately; instead, you go through several steps or "thoughts" to get there. Each thought is a piece of the puzzle.

2. Tree Structure: These thoughts are organized in a tree-like structure. The starting thought is the root of the tree, and each subsequent thought branches out from there. This structure allows the model to explore different paths or sequences of thoughts towards the solution.

3. Evaluation and Selection: At each step, the language model generates multiple thought candidates and evaluates how likely each one is to lead to the solution. The best candidates are selected and expanded in the next step. This is similar to how a chess player might consider different moves and their potential outcomes before deciding on the best one.

4. Lookahead and Backtracking: The model uses search algorithms to systematically explore the tree of thoughts. It can "look ahead" to evaluate future steps based on the current thought, and it can "backtrack" to previous thoughts if a certain path doesn't lead to the solution. This allows the model to navigate the tree efficiently and effectively.

5. Adaptation and Learning: Some implementations of ToT use reinforcement learning to train a "controller" that guides the search process. This controller can learn from new data and adapt its strategy over time, allowing the system to improve its problem-solving capabilities even with a fixed language model.

In essence, the Tree of Thoughts theory is about breaking down complex problems into manageable steps, exploring different paths towards the solution, and learning from experience to improve future performance. It's a way to make language models more strategic and adaptable in their problem-solving approach.


***
***
***

### 20 ChatGPT prompt methods:

1. Second-Order Thinking

Prompt: "Apply Second-Order Thinking to assess [my business decision]. Consider not only the immediate consequences but also the second-level consequences that may arise."

2. Pareto Principle (80/20 Rule)

Prompt: "Use the Pareto Principle to evaluate [my business decision]. Focus on the 20% of factors that could be responsible for 80% of the results."

3. First Principle Thinking

Prompt: "Use First Principle Thinking to evaluate [my business decision]. Rethink the problem from the ground up and separate the underlying facts from the assumptions made based on them."

4. Regret Minimization Framework

Prompt: "Use the Regret Minimization Framework to assess [my business decision]. Think long-term and weigh the emotional impact to minimize future regret."

5. Opportunity Costs

Prompt: "Assess [my business decision] by considering the Opportunity Costs. Think about the costs arising from choosing this option against every other option available."

6. The Sunk Cost Fallacy

Prompt: "Assess [my business decision] while avoiding the Sunk Cost Fallacy. Evaluate the decision based on future value, not past costs."

7. Occam's Razor

Prompt: "Apply Occam's Razor to assess [my business decision]. Choose the less complex explanation or option that satisfies the conditions without unnecessary multiplication."

8. Systems Thinking

Prompt: "Use Systems Thinking to assess [my business decision]. View the problem as part of an interconnected system and understand how variables influence one another."

9. Inversion

Prompt: "Utilize Inversion to analyze [my business decision]. Look at the problem from the endpoint instead of the starting point and ask: 'What must I avoid?' rather than 'What do I need to do?'"

10. Leverage

Prompt: "Analyze [my business decision] through the lens of Leverage. Determine how the right lever can amplify my efforts and lead to significant outcomes."

11. Circle of Competence

Prompt: "Apply the Circle of Competence to analyze [my business decision]. Make sure the decision aligns with [my areas of expertise]. Straying outside of my circle can lead to poor decisions."

12. Law of Diminishing Returns

Prompt: "Evaluate [my business decision] using the Law of Diminishing Returns. Consider the turning point where additional investments offer less value and costs may rise."

13. Niches

Prompt: "Analyze [my business decision] focusing on Niches. Determine how specialization within a niche can lead to expertise and success in this context."

14. Margin of Safety

Prompt: "Use the Margin of Safety to evaluate [my business decision]. Assume that your assumptions might be wrong and plan with a safety margin to mitigate risks."

15. Hanlon's Razor

Prompt: "Evaluate [my business decision] through Hanlon's Razor. Don't assume ill intent when mistakes can be explained by ignorance or error."

16. Randomness

Prompt: "Evaluate [my business decision] with the concept of Randomness in mind. Remember that not everything follows cause-effect relationships and some outcomes may be random."

17. Critical Mass

Prompt: "Analyze [my business decision] by considering Critical Mass. Recognize if you are at a point where momentum may become self-sustaining."

18. The Halo Effect

Prompt: "Evaluate [my business decision] while considering the Halo Effect. Recognize how impressions in one area can bias judgment in others."

19. Feedback Loops

Prompt: "Analyze [my business decision] through the understanding of Feedback Loops. Consider how actions and reactions within the system can influence subsequent decisions."

20. Scarcity and Abundance Mindset

Prompt: "Evaluate [my business decision] considering both Scarcity and Abundance Mindset. Reflect on how your mindset can influence the decision-making process."


