---
status:
  - learning
type:
  - course-project
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
  - platform/coddy
aliases:
date: 2025-08-31T22:48:00
last_practiced: 2025-08-31T22:48:00
banner: "![[source code image.jpg]]"
banner_icon: 💻
---
# Coddy-Python-Project Bill Split Calculator


<iframe src="https://jandee.vercel.app/ktubbs24" width="100%" height="300" frameborder="0"></iframe>

![[source code image.jpg]]
# Course Practice Note Template
---
tags:  #platform/coddy/project 
date: [[2025-08-31]]
time: 22:47


## 📝 Overview

Designing a basic bill calculator using Python. 

---
## 🔑 Key Concepts

-  Working on a few arithmetic operations pertaining to tip percentage to pay and split a bill
---
## 💻  Project Code Instructions

## Getting Input

The next part of our program is to get input from the program user.

After the welcome message, get two numbers (`float`) from the user that indicate the bill amount and the tip percentage, **in that order**.

```python

print("Bill Split Calculator")
bill_amount = float(input())
tip_percentage = float(input())

````

## Calculating The Tip And Total

Create a bill tip calculator program that follows these steps:

1. Print "Bill Split Calculator" as the program title
2. Get the bill amount from user input
3. Get the tip percentage from user input
4. Calculate the tip amount using the formula: `tip_amount = (tip_percentage / 100) * bill_amount`
5. Add the tip amount to the bill amount to get the total
6. Print the total amount

**Note:** You'll need to convert the input strings to float numbers using `float(input())`

```python

print("Bill Split Calculator")
bill_amount = float(input())
tip_percentage = float(input())
tip_amount = (tip_percentage / 100) * bill_amount
total = tip_amount + bill_amount
print(total)
````

# Splitting The Bill

Now we have a working program that calculates the total bill! The missing part is the splitting feature.

Add to the program a **splitting feature**:

1. It will take an additional number (`int`) from the user that indicates the number of people splitting the bill. (**This will be the third input**)
2. Calculate the amount per person by dividing the total amount by the number of people.
3. In the end, add another print of the amount per person.

**Important:** Your program should output exactly two numbers:

- First: the total amount (including tip)
- Second: the amount per person

**Note:** Print only the numeric values without any additional text or labels to match the expected output format.

```python

print("Bill Split Calculator")
bill_amount = float(input())
tip_percentage = float(input())
num_people = int(input())
tip_amount = (tip_percentage / 100) * bill_amount
total = tip_amount + bill_amount
amount_per_person = total / num_people
print(total)
print(amount_per_person)

```
---

# Formatted Output

The last step of this project is to format the output!

For example, for the following input:

```python
100
5
2
```

Output in the following format:

```python
Bill Split Calculator
Total (including tip): $105.0
Each person pays: $52.5
```

> **Important formatting notes:**
> 
> - The output should be **exactly the same** as shown, including all uppercase letters and symbols
> - **Do not round the numbers** - use Python's default float formatting (no .2f or similar)
> - When numbers are converted to float type, Python will display them with varying decimal places (e.g., 105.0, 52.5, 164.285714285714280)
> - Use f-strings to insert the calculated values directly: `f"${variable_name}"`


```python

print("Bill Split Calculator")
bill_amount = float(input())
tip_percentage = float(input())
num_people = int(input())
tip_amount = (tip_percentage / 100) * bill_amount
total = tip_amount + bill_amount
amount_per_person = float(total / num_people)
print(f"Total (including tip): ${total}")
print(f"Each person pays: ${amount_per_person}")

```

---
## 🔗 Links

- Spaced Repetition Cards For this Topic: [[SR-Python Basic Input Output]]
- Related skill: [[Python-Basic Input Output]] 
- Practice:
	- [[1. Coddy-Python Basic Input Output]]
- Snippet: 
- External: [Link to docs or repo]

