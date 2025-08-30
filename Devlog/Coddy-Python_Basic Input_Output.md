---
status:
  - learning
type:
  - course-practice
language:
  - Python
topic:
  - input/output
platform:
  - Coddy
level:
  - beginner
cards-made:
tags:
  - concept/io/python
  - platform/coddy/io
aliases:
  - input output
date: 2025-08-29T20:57:00
last_practiced: 2025-08-29T21:26:00
---
<iframe src="https://jandee.vercel.app/ktubbs24" width="100%" height="300" frameborder="0"></iframe>
# Coddy-Python_Basic Input_Output
---
tags: #concept/io/python  #platform/coddy/io 
date: [[2025-08-29]]
time: 20:57

## 📝 Overview

- **Input** → getting data from the user (with `input()`)
    
- **Output** → showing data back (with `print()`)


---
## 🔑 Key Concepts

- User input from outside the program would go inside the parenthesis in the input( ). 
- Inputs no matter the input always results as a string type (so string need to be converted or [[Python-Caste]] in  order to do arithmetic operations). 




---
## ⚛️ Code

```python
variable = input("This is the input of someone:")
print(variable)

```


---
## 💻  Practice Examples 

## Write a program for user's age 

Write a program that gets the user's age as input.

The program will output (print) the number of missing **years till 120** (in a specific format, shown below).

For example, for input `25`, the expected output is `"95 years till 120"`.

```python

# this was my first try and I got an error in the console saying "unsupprting operand" and I had to remember that all inputs (even numbers) results as a strong and you can not do operations with strings. 
age = input()
age_difference = 120 - age
print(f"{age_difference} years till 120") = #returns error

# so this is the correct answer to the problem by converting/casting the input to integer (int)
age = int(input())
age_difference = 120 - age 
print(f"{age_difference} years till 120")

# another way that I can write this is the longhand: 

age = input()
age = int(age)
age_difference = 120 - age 
print(f"{age_difference} years till 120")

# I also found out through chatgpt that I could have written the arithmetic within the print!!! 

Another variation is doing the math _right inside the print_, without storing `age_difference` at all:

`age = int(input("Enter your age: ")) 
print(f"{120 - age} years till 120")`

This is shorter, but whether you keep the intermediate variable (`age_difference`) depends on if you’ll reuse it later in the program.

# And then chatgpt suggested that there was a one-liner way of solving the same problem so I tried to do it myself and got it right 🥰 my reply: 

would that be this (if I am wrong do not give me the answer):

age = input( )
print(f"{120 - int(age)} years till 120")

#✅ Nailed it — that’s exactly the one-liner version. You’re taking the string from `input()`, converting it to `int` right inside the f-string, and doing the subtraction inline.
🥰🥰🥰🥰🥰🥰🥰🥰🥰🥰🥰🥰🥰🥰🥰🥰🥰 yayaayayyaayayayayaya!

````

## Instruction

```language

````





---
## ✅ To-Do
#todo
- [ ] 




---
## 📓 Notes

- **Step-by-step (longhand)**
    
- **Cast at assignment (clean middle ground)**
    
- **Do math directly in `print`**
    
- **Full one-liner 



---
## 🔗 Links

- Spaced Repetition Cards For this Topic: [link to the page where all practice questions go for this code]
- Related skill: [[3-Skills/Languages/Python.md]]
- Practice:
	- [[1-Practice/Course Practice/Coddy/Python/Loops.md]]
- Snippet: ![[4-Library/Snippets/Python/for_loops.md]]
- External: [Link to docs or repo]

