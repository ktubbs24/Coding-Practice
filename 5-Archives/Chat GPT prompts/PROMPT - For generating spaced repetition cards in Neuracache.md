---
date: 2025-09-01T17:47:00
status:
  - archived
type:
  - ChatGPT-prompt
tags:
  - chatgpt/prompts
---
# PROMPT - For generating spaced repetition cards in Neuracache
---
date: [[2025-09-01]]
time: 17:46
tags: #chatgpt/prompts

**Prompt Template:**


"I want to make spaced repetition flashcards for coding practice to sync with the Neurocache app via my Obsidian notes vault. Please generate flashcards in the following format:

- Each card begins with a line containing the card tag (e.g., `#card #card/io/python` or make the second tag fit the concept or topic ie if you have cards that fit JavaScript variables go ahead and change the second tag from #card/io/python to #card/variables/javascript) immediately followed by the question on the next line with no extra blank line in between.

- The question is plain text (not a heading) and should be complete and clear for practice and written in a way where I as a beginner can understand it. 

- After the question, insert a line with three dashes `---` as a separator.

- Then provide the Python (or whatever language that fits the codebass) code answer enclosed inside a Python code block (or whatever language that fits the codebass) (using triple backticks with `and the appropriate language for the code`).

- After the answer block, add another line with three dashes `---` as a separator to separate between that previous answer and the next question card. 

Make sure no blank lines exist between the question and the card tag line or between question and the separator.

Please format the output exactly as specified so I can copy and paste directly into Obsidian for syncing to NeuraCache."

Here is an example of what I need the cards to look like in markdown:

#card #card/io/python (or whatever langauge or concept that fits for the second tag)

So the card would look like:

#card #card/io/python
This will be where you word the question but I don’t want you to write the word question.

---
This is the answer or code block here 
```python 
Some code 
```
 

---


Generate cards for common Python coding exercises such as input and output, arithmetic operations, string manipulations, and control flow based on typical beginner and intermediate challenges.



### See also: 
- 
---