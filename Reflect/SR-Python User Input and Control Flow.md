---
date: 2025-09-06T00:34:00
status:
  - reflecting
type:
  - flashcards
level:
  - beginner
language:
  - Python
topic:
  - while loops
  - operations
  - input/output
---
# SR-Python User Input and Control Flow
---
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


# ✌️Two-Sided Cards (code) +

#card #card/input-validation/python #card/while-loops/python #card/conditionals/python #card/logical-operators 
# Python Practice Flashcards

## Card 1

Write a Python program that takes an integer input (`0` or `1`) and outputs `"True"` for `1` and `"False"` for `0`.

```python
user = int(input())
if user == 1:
    print("True")
else:
    print("False")
```

---

## Positive/Negative Check with Validation

## Write a Python program that takes an integer input and outputs `"Positive"` if `> 0` or `"Negative"` if `< 0`. If the input is `0`, prompt with `"Enter a non-zero integer!"` until a non-zero input is received.

```python
user = int(input("Enter a non-zero integer: "))
while user == 0:
    print("Enter a non-zero integer!")
    user = int(input("Enter a non-zero integer: "))
if user > 0:
    print("Positive")
else:
    print("Negative")
```

---

## Card 2

Write a Python program that takes an integer input and outputs `"Even"` if even or `"Odd"` if odd. If the input is `<= 0`, prompt with `"Enter a positive integer!"` up to 3 times, then output `"Too many invalid attempts!"` if invalid after 3 tries.

```python
user = int(input("Enter a positive integer: "))
attempts = 0
while user <= 0 and attempts < 3:
    print("Enter a positive integer!")
    user = int(input("Enter a positive integer: "))
    attempts += 1
if attempts == 3 and user <= 0:
    print("Too many invalid attempts!")
else:
    if user % 2 == 0:
        print("Even")
    else:
        print("Odd")
```

---

## Yes/No Input Validator

## Write a Python program that takes a single character input (`Y` or `N`) and outputs `"Yes"` for `Y` or `"No"` for `N`. If the input is not `Y` or `N`, prompt with `"Please enter Y or N!"` until valid.

```python
user = input("Enter Y or N: ")
while user != "Y" and user != "N":
    print("Please enter Y or N!")
    user = input("Enter Y or N: ")
if user == "Y":
    print("Yes")
else:
    print("No")
```

---

## Card 3

Write a Python program that takes an integer input and outputs the number if it’s between `1` and `5` (inclusive). If not, prompt with `"Please enter a number between 1 and 5!"` until valid.

```python
user = int(input("Enter a number between 1 and 5: "))
while user < 1 or user > 5:
    print("Please enter a number between 1 and 5!")
    user = int(input("Enter a number between 1 and 5: "))
print(user)
```

---

## Pass/Fail Grade Validator

## Write a Python program that takes an integer input (`0` or `1`) and outputs `"Pass"` for `1` and `"Fail"` for `0`. If the input is not `0` or `1`, prompt with `"Enter 0 or 1!"` until valid.

```python
user = int(input("Enter 0 or 1: "))
while user != 0 and user != 1:
    print("Enter 0 or 1!")
    user = int(input("Enter 0 or 1: "))
if user == 1:
    print("Pass")
else:
    print("Fail")
```

---

## Vowel/Consonant Checker

## Write a Python program that takes a single lowercase letter input and outputs `"Vowel"` if the letter is a vowel (`a`, `e`, `i`, `o`, `u`) or `"Consonant"` otherwise. If the input is not a lowercase letter, prompt with `"Enter a lowercase letter!"` until valid.

```python
user = input("Enter a lowercase letter: ")
while not user.islower() or user not in "aeiou":
    print("Enter a lowercase letter!")
    user = input("Enter a lowercase letter: ")
if user in "aeiou":
    print("Vowel")
else:
    print("Consonant")
```

---

## Card 4

Write a Python program that takes an integer input and outputs `"High"` if `>= 10` or `"Low"` if `< 10`. If the input is `0`, prompt with `"Enter a non-zero integer!"` until a non-zero input is received.

```python
user = int(input("Enter a non-zero integer: "))
while user == 0:
    print("Enter a non-zero integer!")
    user = int(input("Enter a non-zero integer: "))
if user >= 10:
    print("High")
else:
    print("Low")
```

---

## Day/Night Input Validator

## Write a Python program that takes a single character input (`D` or `N`) and outputs `"Day"` for `D` or `"Night"` for `N`. If the input is not `D` or `N`, prompt with `"Enter D or N!"` until valid.

```python
user = input("Enter D or N: ")
while user != "D" and user != "N":
    print("Enter D or N!")
    user = input("Enter D or N: ")
if user == "D":
    print("Day")
else:
    print("Night")
```

---

## Card 5

Write a Python program that takes an integer input and outputs `"Valid"` if it’s between `10` and `20` (inclusive). If not, prompt with `"Enter a number between 10 and 20!"` until valid.

```python
user = int(input("Enter a number between 10 and 20: "))
while user < 10 or user > 20:
    print("Enter a number between 10 and 20!")
    user = int(input("Enter a number between 10 and 20: "))
print("Valid")
```


## Card 1

Does Python support multiple lines of code inside a loop?

```python
Yes, Python supports multiple lines of code inside any loop (e.g., while, for), as long as they are properly indented.
```

---

## Card 2

Can conditional statements (`if`, `elif`, `else`) be nested inside loops in Python?

```python
Yes, conditional statements (`if`, `elif`, `else`) can be freely nested inside loops, with proper indentation.
```

---

## Card 3

What is the correct logical AND operator in Python, and how does it differ from JavaScript?

```python
Python uses `and` (lowercase) for the logical AND operator. JavaScript uses `&&`. `AND` is not valid in Python.
```

---

## Card 4

What is the correct inequality operator in Python, and is `!==` valid?

```python
Python uses `!=` for inequality. `!==` is not valid in Python.
```

---

## Card 5

Can you put a condition or code on the `else` line in a Python `if-else` statement?

```python
No, the `else` line in a Python `if-else` statement cannot have a condition or code; it must be `else:` only.
```

---

## Card 6

What happens if a user enters a non-numeric input when a Python program expects a number with `int(input())`?

```python
A `ValueError` occurs if a user enters a non-numeric input (e.g., "a") when using `int(input())`. It does not cause a `SyntaxError`.
```

---

## Card 7

What error occurs in this code if the user enters a non-numeric input?

```python
user = int(input("Enter a number: "))
#an error will run if user enters anything other than a number
```

```python
A `ValueError` will occur if the user enters a non-numeric input (e.g., "a").
```

---

## Card 8

Write a Python program that takes an integer input (`0` or `1`) and outputs `"True"` for `1` and `"False"` for `0`.

```python
user = int(input())
if user == 1:
    print("True")
else:
    print("False")
```

---

## Positive/Negative Check with Validation

## Write a Python program that takes an integer input and outputs `"Positive"` if `> 0` or `"Negative"` if `< 0`. If the input is `0`, prompt with `"Enter a non-zero integer!"` until a non-zero input is received.

```python
user = int(input("Enter a non-zero integer: "))
while user == 0:
    print("Enter a non-zero integer!")
    user = int(input("Enter a non-zero integer: "))
if user > 0:
    print("Positive")
else:
    print("Negative")
```

---

## Yes/No Input Validator

## Write a Python program that takes a single character input (`Y` or `N`) and outputs `"Yes"` for `Y` or `"No"` for `N`. If the input is not `Y` or `N`, prompt with `"Please enter Y or N!"` until valid.

```python
user = input("Enter Y or N: ")
while user != "Y" and user != "N":
    print("Please enter Y or N!")
    user = input("Enter Y or N: ")
if user == "Y":
    print("Yes")
else:
    print("No")
```

---

## Card 9

Write a Python program that takes an integer input and outputs the number if it’s between `1` and `5` (inclusive). If not, prompt with `"Please enter a number between 1 and 5!"` until valid.

```python
user = int(input("Enter a number between 1 and 5: "))
while user < 1 or user > 5:
    print("Please enter a number between 1 and 5!")
    user = int(input("Enter a number between 1 and 5: "))
print(user)
```

---

## Pass/Fail Grade Validator

## Write a Python program that takes an integer input (`0` or `1`) and outputs `"Pass"` for `1` and `"Fail"` for `0`. If the input is not `0` or `1`, prompt with `"Enter 0 or 1!"` until valid.

```python
user = int(input("Enter 0 or 1: "))
while user != 0 and user != 1:
    print("Enter 0 or 1!")
    user = int(input("Enter 0 or 1: "))
if user == 1:
    print("Pass")
else:
    print("Fail")
```

---

## Vowel/Consonant Checker

## Write a Python program that takes a single lowercase letter input and outputs `"Vowel"` if the letter is a vowel (`a`, `e`, `i`, `o`, `u`) or `"Consonant"` otherwise. If the input is not a lowercase letter, prompt with `"Enter a lowercase letter!"` until valid.

```python
user = input("Enter a lowercase letter: ")
while not user.islower() or user not in "aeiou":
    print("Enter a lowercase letter!")
    user = input("Enter a lowercase letter: ")
if user in "aeiou":
    print("Vowel")
else:
    print("Consonant")
```

---

## Card 10

Write a Python program that takes an integer input and outputs `"High"` if `>= 10` or `"Low"` if `< 10`. If the input is `0`, prompt with `"Enter a non-zero integer!"` until a non-zero input is received.

```python
user = int(input("Enter a non-zero integer: "))
while user == 0:
    print("Enter a non-zero integer!")
    user = int(input("Enter a non-zero integer: "))
if user >= 10:
    print("High")
else:
    print("Low")
```

---

## Day/Night Input Validator

## Write a Python program that takes a single character input (`D` or `N`) and outputs `"Day"` for `D` or `"Night"` for `N`. If the input is not `D` or `N`, prompt with `"Enter D or N!"` until valid.

```python
user = input("Enter D or N: ")
while user != "D" and user != "N":
    print("Enter D or N!")
    user = input("Enter D or N: ")
if user == "D":
    print("Day")
else:
    print("Night")
```

---

## Card 11

Write a Python program that takes an integer input and outputs `"Valid"` if it’s between `10` and `20` (inclusive). If not, prompt with `"Enter a number between 10 and 20!"` until valid.

```python
user = int(input("Enter a number between 10 and 20: "))
while user < 10 or user > 20:
    print("Enter a number between 10 and 20!")
    user = int(input("Enter a number between 10 and 20: "))
print("Valid")
```

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

### Links to Course Notes Related to SR-Python User Input and Control Flow:
- Coddy: [[Coddy-]]
- freeCodeCamp: [[freeCodeCamp-]]
- W3Schools: [[W3Schools-]]
- CodeAcademy: [[CodeAcademy-]]
- Sololearn: [[Sololearn-]]

### Links to Extra Practice and Problems For SR-Python User Input and Control Flow:
- 



---
### See also: 
- 
---
