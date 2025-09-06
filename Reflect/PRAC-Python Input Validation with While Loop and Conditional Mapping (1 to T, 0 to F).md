---
status:
  - mastered
type:
  - course-practice
language:
  - Python
topic:
  - input/output
  - while loops
platform:
  - Coddy
level:
  - beginner
cards-made: true
tags:
  - practice/while-loops/python
  - practice/if-else/python
  - practice/conditions/python
aliases:
date: 2025-09-05T22:10:00
last_practiced: 2025-09-06
banner: "![[source code image.jpg]]"
banner_icon: 💻
---
# PRAC-Python Input Validation with While Loop and Conditional Mapping (1 to T, 0 to F)

<iframe src="https://jandee.vercel.app/ktubbs24" width="100%" height="300" frameborder="0"></iframe>

---
tags: #topic/while-loops/python #topic/input/python #topic/print/python #platform/coddy 
date: [[2025-09-05]]
time: 00:05
## 🧪 Write a program that will output T or F based on user input

Write a program that gets an input from the user, a number, `1` or `0`.
The program will output `"T"` if the input is 1 and `"F"` otherwise.
> Remember! you can cast the input to number using `int()`
### First Attempt 
```python

# comments are suggestions from chatgpt to corret code

user = int(input("Enter the number 1 or 0:  ")) #come up with a way to prevent a ValueError if the user does not enter the numbers 1 or 0 and enters a letter instead  

if user == 1: 
	print("T")
else user == 0: #the else block does not include a condition
	print("F")
print("Invalid entry. Enter either 1 or 0") #this will print regardless out the output because it is outside the if-else structure

```

---
### Second Attempt 
```python
user = int(input("Enter the number 1 or 0:  "))
if user !== 1 OR user !== 0:  #use AND instead of OR because you want both conditions to be true. Do not use !== because Python uses != and JS uses !==.....my mistake from switching from JavaScript 😝
	print("Invalid entry. Enter either 1 or 0!")
if user == 1: 
	print("T")
else:
	print("F")
```

#### personal notes on my code: 

- Realizing that the second line would check if the user input is either 1 or 0 but the code would still possibly run if someone were to enter in the number 5 or any other number outside of 1 or 0. 
---
### Third Attempt 
```python
user = int(input("Enter the number 1 or 0:  "))

while user != 1 AND  user != 0:  #use `and` not `AND` in Python. 
	print("Invalid entry. Enter either 1 or 0!")
	user = int(input("Enter the number 1 or 0:  "))
print(user) #was good enough for debugging but this is not asking for this print in the instructions.

if user == 1:  #these if statements execute the answer to the problem but I need to simplify this to an if else statement since the only output from the user after the while loop would have to be 1or 0. 
	print("T")

if user == 0: 
	print("F")
```

#### personal notes on my code: 
I decided that in order to make sure that the input from the user needs to be 1 or 0 that I need to do a while loop instead of just an if-else statement because the while loop would force the user to input 1 or 0 according to the `while` condition making the input be 1 or 0 to fulfill the if-else statements after. 

I am still learning on if-else statements and thought that having two if statements would be necessary but realized that it does not since the only other option to print for anything if the user input weren't 1 is 0 by default again due to the while loop statement before. 

---
### Fourth & Final Attempt!!! 🎉
.... After putting the bottom code back in Coddy and ran it...it wanted me to run the simpler version even though both get the same results so I am proud of myself for figuring this out but still a little annoyed....😩

```python 
# this is the code that was accepted in Coddy  a simpler version over the one below: 
user = int(input( ))

if user == 1:
	print("T")
else:
	print("F")
```

```python 
user = int(input("Enter the number 1 or 0:  "))
while user != 1 and  user != 0:  
	print("Invalid entry. Enter either 1 or 0!")
	user = int(input("Enter the number 1 or 0:  "))	
if user == 1: 
	print("T")
else: 
	print("F")
```

#### Line-by-Line Analysis (the longhand version)

**Line 1: `code_line_here`**  
   - Explanation:  
   - Details: 
   - Potential pitfalls: 

**Line 2: `code_line_here`**  
   - Explanation: 
   - Details: 
   - Potential pitfalls: 


**Line 3: `code_line_here`**  
   - Explanation: 
   - Details: 
   - Potential pitfalls: 


**Line 4: `code_line_here`**  
   - Explanation: 
   - Details: 
   - Potential pitfalls: 

**Line 5: `code_line_here`**  
   - Explanation: 
   - Details: 
   - Potential pitfalls: 


**Line 6: `code_line_here`**  
   - Explanation: 
   - Details: 
   - Potential pitfalls: 


**Line 7: `code_line_here`**  
   - Explanation: 
   - Details: 
   - Potential pitfalls: 

**Line 8: `code_line_here`**  
   - Explanation: 
   - Details: 
   - Potential pitfalls: 

---
## 🔗 Links

- Spaced Repetition Cards For this Topic: [[SR-Python User Input and Control Flow]]


