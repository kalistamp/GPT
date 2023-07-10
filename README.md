# *SOME PROMPT FORMATS AND EXPLAINATIONS:*

### Standard GPT Prompt Format: 

[IMAGE](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*OrfhOZhi-PmOjUY-cLI0_g.png)

* Task description
* Examples
* Prompt, main question

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
  

***
***
***

### Prompts: 

* https://prompts.chat/ - [Ex.] Act as a lnux terminal...

***

### Sources:

* PROMPT ENG. TOOL - https://github.com/mshumer/gpt-prompt-engineer
* THE PROMPT ENG. GUIDE - https://www.promptingguide.ai/
* PROMPT ENG. WEBSITE - https://learnprompting.org/docs/prompt_hacking/injection
* PROMPT BOOK - https://heystacks.com/doc/1273/the-chatgpt-prompt-book-lifearchitectai-rev

***

### GPT Githubs:

* AWESOME PROMPT ENG. LIST: https://github.com/promptslab/Awesome-Prompt-Engineering
* https://github.com/mshumer
