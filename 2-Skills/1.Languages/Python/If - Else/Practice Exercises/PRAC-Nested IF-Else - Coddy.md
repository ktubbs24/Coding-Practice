---
status:
  - learning
type:
  - course-practice
language:
topic:
platform:
level:
  - beginner
cards-made:
tags:
aliases:
date:
last_practiced:
  "{ date }":
banner: "![[source code image.jpg]]"
banner_icon: 💻
---


<iframe src="https://jandee.vercel.app/ktubbs24" width="100%" height="300" frameborder="0"></iframe>

# PRAC-Nested IF-Else - Coddy
---
tags: #topic/ #platform/ 
date: [[2025-10-03]]
time: 18:07
## ⚛️ Code

```python 
age = 18
title = "None"
allowed_to_drink = False
if age >= 18:
    title = "Adult"
    if age >= 21:
        allowed_to_drink = True
    else:
        allowed_to_drink = False
else:
    title = "Minor"
```

In this example, the second if-else only executes when the first condition is `True`

---
## 💻  Practice Examples 

## Instruction 

Write a program that determines eligibility for a movie based on age and parental guidance.

Your program should:

1. Create a variable `age` and assign it a value from input. 
2. Create a variable `with_parent` and assign it a True/False value from input. 
3. Create a variable named `message` with the value of `"None"`. 
4. Use nested if-else to determine what string to put in `message`: 
    - If age is 18 or older, set `"You can watch any movie"`.
    - If age is under 18: 
        - If with_parent is True, set `"You can watch PG-13 movies"`.
        - If with_parent is False, set `"You can only watch G-rated movies"`.

```python
age = int(input())
with_parent = input() == "true" #will this automatically change to True when in the compiler? 
message = "None"

if age >= 18:
	message = "You can watch any movie"
if age < 18: 
    if with_parent == True: 
	    message = "You can watch PG-13 movies"
    if with_parent == False: 
        message = "You can only watch G-rated movies"
print(message)
````

### Personal Comments 

I tried to rewrite this so that it was not a bunch of if statements logically written but is a program that follows the instructions using if-else. 

Also this code given for the problem:
```python 
with_parent = input() == "true" #will this automatically change to True when in the compiler? 
```

will only work if the user inputs lower case `true` as explained by chatgpt: 

Good question 👌
This part can be confusing at first, so let’s break it down carefully:

Your original line was:

```python
with_parent = input() == "true"
```

Let’s say the program runs and the user types:

```
true
```

➡️ What happens:

* `input()` returns the string `"true"`.
* `"true" == "true"` evaluates to `True` (Python’s boolean value).
* So `with_parent` is assigned `True`.

👉 That means your `if with_parent == True:` and `if with_parent == False:` statements both work exactly as intended, because `with_parent` is now literally a **boolean**, not a string anymore.

---

But here’s the important subtlety 👇

If the user typed:

```
True
```

(with a capital “T”) or

```
TRUE
```

or

```
yes
```

or anything else...

Then:

* `"True" == "true"` → `False`
* `"TRUE" == "true"` → `False`
* `"yes" == "true"` → `False`

So `with_parent` would be `False` in all those cases, and your code would **still run**, but maybe not give the result you expected, depending on what was typed.

---

### Why it “still worked” in your test:

Most likely, when you tested it in the IDE, you typed **exactly** `true` (all lowercase) for the input.
That’s why it matched `"true"` exactly, giving you `True` or `False` properly, and your `if` checks worked.

---

### ⚡ Summary:

* Your code *works* as long as the input matches `"true"` exactly.
* It doesn’t “automatically” convert arbitrary strings like `"True"` to boolean — it’s the equality comparison that’s doing the work.
* That’s why `.lower()` is often used:

  ```python
  with_parent = input().lower() == "true"
  ```

  This way, `"TRUE"`, `"True"`, or `"true"` would all return `True`.

So another attempt: 
```python 
if age >= 18:
    message = "You can watch any movie"
    if age < 18: 
        if with_parent == True:
            message = "You can watch PG-13 movies"
        else: 
            message = "You can only watch G-rated movies"
print(message)
```

Some notes from chatgpt: 

Ah 👌 — I see exactly what you’re testing here.

This structure **looks like** it’s nested because the second `if` is indented under the first `if`, but logically, there’s a **problem**:

```python
if age >= 18:
    message = "You can watch any movie"
    if age < 18:   # 👈 this will never run if age >= 18 is True
        ...
```

You’re checking `if age < 18` **inside** the block that only runs when `age >= 18` is true — which can never happen at the same time.

This is what’s called a ==**mutually exclusive condition**== placed inside another, so the inner `if` is effectively ==**dead code**==.

👉 The nesting you want isn’t:
`if age >= 18`
→ `if age < 18` (inside)

Instead, it should be:
`if age >= 18:`
→ `else:`
→→ `if with_parent:`
→→ `else:`

That’s the shape you’re aiming for.

So: the problem with your snippet isn’t syntax — it’s **logic flow**.
No syntax error will appear, but only the “You can watch any movie” branch will ever run if `age >= 18`, because the `if age < 18` inside will never be true.


So let me try again : 

```python 

age = int(input())
with_parent = input() == "true" 
message = "None"

if age >= 18:
    message = "You can watch any movie"
    if age < 18:  #found out that this is redundant because by default the program will know that anything under "else" will be less than 18 (age < 18) so no need to write this here.
        if with_parent == True:
            message = "You can watch PG-13 movies"
        else: 
            message = "You can only watch G-rated movies"
print(message)
```

So I rewrote the code again and discovered that you can indent `if` statements inside of `else` statements meaning that I fulfilled what the problem asked!!!!: 

```python 
if age >= 18:
    message = "You can watch any movie"
else: 
    if with_parent == True:
        message = "You can watch PG-13 movies"
    else: 
        message = "You can only watch G-rated movies"
print(message)
```

^bb649b


- So I ended up asking if I could place `if` statements in an else block and I can: 
	- [[CHAT-Can I place IF statements in else block in python]]
-  And I also asked what is the main purpose for using this form of if-else nesting over if-elif or just multiple if-else statements in a program? 
	- [[CHAT-What is the point of using if statements nested in else blocks in Python]]
## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Instruction

```language

````

## Final Code

```language

````


---
## ✅ To-Do
#todo
- [ ] 




---
## 📓 Notes





---
## 🔗 Links

- Spaced Repetition Cards For this Topic: [[SR-]]
- Snippet: 
- External: [Link to docs or repo]


