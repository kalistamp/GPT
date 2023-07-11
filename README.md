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

### Prompts: 

* https://prompts.chat/ - [Ex.] Act as a lnux terminal...

***

### Sources:

* PROMPT ENG. TOOL - https://github.com/mshumer/gpt-prompt-engineer
* TOOLS - https://www.promptingguide.ai/tools
* THE PROMPT ENG. GUIDE - https://www.promptingguide.ai/
* PROMPT ENG. WEBSITE - https://learnprompting.org/docs/prompt_hacking/injection
* AI NEWS - https://www.mlyearning.org/

***

### GPT Githubs:

* AWESOME PROMPT ENG. LIST: https://github.com/promptslab/Awesome-Prompt-Engineering
* https://github.com/mshumer
