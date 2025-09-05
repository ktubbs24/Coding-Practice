---
date: 2025-09-04T19:24:00
status:
  - review
type:
  - flashcards
level:
  - beginner
language:
  - Python
topic:
  - while loops
---

# SR-Python While Loops

# ♦️ Regular Cards (regular)+
---
## card

Question `# card`
Answer

---
## card

Question `# card`
Answer

---

## card

Question `# card`
Answer

---

## card

Question `# card`
Answer

---

## card

Question `# card`
Answer

---

## card

Question `# card`
Answer

---

## card

Question `# card`
Answer

---

## card

Question `# card`
Answer

---

## card

Question `# card`
Answer

---

## card

Question `# card`
Answer

---

## card

Question `# card`
Answer

---

## card

Question `# card`
Answer

---

## card

Question `# card`
Answer

---

## card

Question `# card`
Answer

---

## card

Question `# card`
Answer

---

## card

Question `# card`
Answer

---



# ♦️ Regular Cards (code) +
---
## card

Question `# card`
```language


```

---

## card

Question `# card`
```language


```

---
## card

Question `# card`
```language


```

---
## card

Question `# card`
```language


```

---
## card

Question `# card`
```language


```

---
## card

Question `# card`
```language


```

---
## card

Question `# card`
```language


```

---
## card

Question `# card`
```language


```

---
## card

Question `# card`
```language


```

---
## card

Question `# card`
```language


```

---
## card

Question `# card`
```language


```

---
## card

Question `# card`
```language


```

---
## card

Question `# card`
```language


```

---
## card

Question `# card`
```language


```

---
## card

Question `# card`
```language


```

---
## card

Question `# card`
```language


```

---



# ✌️ Two-Sided Cards (regular) +

## card

`# card`
Question 


- - - 
Answer 

- - -

## card

`# card`
Question 


- - - 
Answer 

- - -
## card

`# card`
Question 


- - - 
Answer 

- - -
## card

`# card`
Question 


- - - 
Answer 

- - -
## card

`# card`
Question 


- - - 
Answer 

- - -
## card

`# card`
Question 


- - - 
Answer 

- - -
## card

`# card`
Question 


- - - 
Answer 

- - -
## card

`# card`
Question 


- - - 
Answer 

- - -
## card

`# card`
Question 


- - - 
Answer 

- - -
## card

`# card`
Question 


- - - 
Answer 

- - -
## card

`# card`
Question 


- - - 
Answer 

- - -
## card

`# card`
Question 


- - - 
Answer 

- - -


# ✌️Two-Sided Cards (code) +8

## While Loop Condition

#card #card/while-loops/python
Explain the purpose of: `while number >= 2.5:` 
in the context of a program that divides a number by 3 until it’s less than 2.5. Write the code and answer and have it print the result. 

---
```python
number = float(input())
while number >= 2.5:
    number /= 3
print(number)
```
Explanation: This line starts a while loop that continues as long as the variable number is greater than or equal to 2.5. It checks the condition before each iteration to decide whether to execute the loop body.

---

## Division Operation in Loop

#card #card/while-loops/python
What does `number /= 8` do inside a while loop, and how else could it be written?

---
Explanation: It divides the variable number by 8 and stores the result in the number variable. 
- It can also be written as `number = number / 8.` 
- This operation is executed each time the while loop runs if the condition number >= 2.5 is true.

---
## Print Statement Placement

#card #card/while-loops/python #card/print/python
What is the purpose of making sure that a `print(variable)` statement  is placed *outside* a while loop (not indented but outdented) in a program?

---

The `print(variable)` statement is outside the while loop to print only after the condition for the while loop isn’t met anymore printing the final result. 

---

## Potential Pitfall: Incorrect Division

#card #card/while-loops/python #card/arithmetic-operations #card/debugging 
What happens if you write `number = 3` instead of `number /= 3` in a while loop?

---
Writing `number = 3` sets number to 3 in each loop iteration, ignoring the user’s input and the division operation. This causes the loop to run indefinitely (infinite loop) if number starts ≥ 2.5, or it stops immediately if number < 2.5, without performing the required divisions.

---

## Potential Pitfall: Missing Variable Update

#card #card/while-loops/python #card/debugging/python #card/arithmetic-operations 
What goes wrong if you write `number / 3` instead of `number /= 3` in the while loop?

---
Writing `number / 3` performs the division but doesn’t store the result back in `number`. The variable `number` remains unchanged, causing an infinite loop if the initial input is ≥ 2.5, as the condition number >= 2.5 never becomes false.

---

## Input Handling in Different Environments

#card #card/while-loops/python
How should the input line for python be adjusted when writing a program in an online IDE versus a local environment like Coddy?

---
In an online IDE, use 
`number = float()` 
or `number = {a number} ie number = 13` 
instead of `number = float(input())`
as the input is often provided automatically.
In a local environment like Coddy, 
`number = float(input())` is used to prompt the user for input.

---
## Program Output Goal

#card #card/while-loops/python #card/input/python 
 What is the goal of the program that uses a while loop to divide a float input by 6 as long as the number is ≥ 2.5, and prints the first number that is < 2.5 when the loop stops.? 
 
 Explain after writing the problem out. 
 
---
```python
number = float(input())
while number >= 2.5:
    number /= 6
print(number)

```

Explanation: The program takes a float input, divides it by 6 repeatedly as long as the number is ≥ 2.5, and prints the first number that is < 2.5 when the loop stops.

---

## Input and Float Conversion

#card #card/while-loops/python #card/input/python 
What does number = float(input()) do in a Python while loop program that divides a number by 3 if it meets the condition where the number is less than 5? 
Right the answer to these instructions and then explain what it does. 

---
```python
number = float(input())
while number < 5:
    number /= 3     
```
Explanation: It takes a user input as a string, converts it to a float, and stores it in the variable number. This allows the program to work with decimal numbers for division in the while loop.

---


## card

`# card`
Question 


- - - 
Answer

```language


```
- - -
## card

`# card`
Question 


- - - 
Answer

```language


```
- - -
## card

`# card`
Question 


- - - 
Answer

```language


```
- - -
## card

`# card`
Question 


- - - 
Answer

```language


```
- - -
## card

`# card`
Question 


- - - 
Answer

```language


```
- - -
## card

`# card`
Question 


- - - 
Answer

```language


```
- - -
## card

`# card`
Question 


- - - 
Answer

```language


```
- - -
## card

`# card`
Question 


- - - 
Answer

```language


```
- - -
## card

`# card`
Question 


- - - 
Answer

```language


```
- - -
## card

`# card`
Question 


- - - 
Answer

```language


```
- - -
## card

`# card`
Question 


- - - 
Answer

```language


```
- - -
## card

`# card`
Question 


- - - 
Answer

```language


```
- - -
## card

`# card`
Question 


- - - 
Answer

```language


```
- - -


# 1️⃣  One-Liner Cards +
---
## card
Question : Answer `# card `

---
## card
Question : Answer `# card `

---
## card
Question : Answer `# card `

---
## card
Question : Answer `# card `

---
## card
Question : Answer `# card `

---
## card
Question : Answer `# card `

---
## card
Question : Answer `# card `

---

# 🚀  Spaced Repetition Cards 
*(this is just for memory retention of certain concepts)*

---

## card

`# spaced `
Content

--- 

## card

`# spaced `
Content

--- 

## card

`# spaced `
Content

--- 

## card

`# spaced `
Content

--- 

## card

`# spaced `
Content

--- 

## card

`# spaced `
Content

--- 

## card

`# spaced `
Content

--- 

## card

`# spaced `
Content

--- 

## card

`# spaced `
Content

--- 

## card

`# spaced `
Content

--- 


# 🔗 Related Links 

### Links to Course Notes Related to SR-Python While Loops:
- Coddy: [[Coddy-]]
- freeCodeCamp: [[freeCodeCamp-]]
- W3Schools: [[W3Schools-]]
- CodeAcademy: [[CodeAcademy-]]
- Sololearn: [[Sololearn-]]

### Links to Extra Practice and Problems For SR-Python While Loops:
- 



---
### See also: 
- 
---
# SR-Python While Loops
