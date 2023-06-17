### What is python?
- An high-level and interpreted programming language that is used to code programs.

#### Characteristics 🐸
** A High-level Language**:
    - (source code that must be translated to machine level code for execution)
**Interpreted Language: **
    - Executed line by line until it meets an error
**Interactive Interpreter:**
    - Can test lines of code on its interpreter
**Object-Oriented **

### Commenting
    - A way to leave human-readable notes for the reader. Often used to explain your coding and variable naming philosophy
    
### Documentation
     - The multi-line commenting feature will often used to describe your self-made functions or objects
     - Not often used for other types of code.

### Variables
`   -  In Python, we can assign different types of built-in data type to a label, which we call a “variable”
    - We use singular equal sign to assign a value to a variable.

### Naming Conventions
    - **Avoid** using single letters to denote variable names
    - **Avoid** starting variable names with numbers
    - Variable names **should** be short, but reflective of what the variable contains
    - Spaces should be avoided and multi-word variable should use either **camelCasing or under_scores** 
                - (camelCasing is where different words are separated by capitalization)
    - Avoid using special/reserved keywords of a programming language
    - Don’t start variable names with capitals

### input()
    - The input function halts the program until an input has been entered into the program.
    - The input function can have an empty parameter; however, we can add string messages to output before we receive an input
            - This is called a prompt

### Conditionals
    - Any non-zero and non-null values evaluate to True
    - 1 is True
    - 0 is False
    
#### if statements
    - one of the most common ways to handle conditional
    - if statements will execute its own block of code iff its own boolean expression evaluates to **True**.
    
#### if else statements
    - when the if’s boolean expression is False, the else’s code block will be executed
          - This is very powerful for binary decisions.
    - also very clean coding practice to make sure that the program knows how to handle
      situations when the boolean_expression evaluates to False.
#### if elif else
    - Sometimes there can be multiple conditionals rather than a binary condition
        -  Your Boolean expressions should all be related to each other. 
            - If not... just start a new if statement.
### range()
    - A function that generates a sequence of numbers in an arithmetic progression. 
        - range(start,end-step,step)
### Iterations
    - Iteration: the act of repeating a mathematical or computational process.
#### Why we iterate 🐸
    - Generate unbounded sequence of outcomes
    - Approach a desired goal/target/result

**All For Loops can be turned to While Loops, but not the other way around**

#### while loop
    - A conditional based iteration that repeats its block of code iff its boolean expression is **true**.
##### Infinite while loop
    - Infinite While Loops is an iteration technique that **never** ends. 
    - The boolean expression in the while loop is never affected by the while loop code block, and it always evaluates to True.
        - WHILE LOOP NEVER BECOMES FALSE
            - useful for gaming 
 ##### while else 
    - Python 3 also also allows while … else. 
    - The else’s code block only executes **if** the while’s boolean expression evaluates to False.
    
 ``` python 
  num = 10
  while num != 10:
	print(“The number is:”, num)
	num -= 1
  else:
	print(“The number is now:”, num)
  ```
  ##### flag based while loops
    - Flag: a value that acts as a signal for a function or process
   ``` python
num = 2
flag = True
while flag:
	print(num)
	num **= 2
	user_input = input(‘Exit? (Y/N): ‘)
	if user_input in ‘Yy’:
		flag = False
   ```
   #### for loops
    -  a iteration through items within a sequence. The variable will hold the item value for each iteration step.

### Functions
    - a block of organized, reusable code that is usually used to perform a **single** and **related action**.
            - There are built-in functions for languages
            - Most languages support you to create functions
                    - Similar Concepts or terms: methods, subroutines, procedures
#### Programming function 🐸
    - single input can be mapped to **different/multiple** output. 
    - Think of it as self contained module of code that is meant to accomplish a specific task
    
#### How does it work? 
    - A program may execute a function call
    - The program enters the function
    - All instructions within the function will executed from top to bottom
    - The program leaves the function and returns to the program’s flow
    - Any data computed and RETURNED by the function is used by the program

#### Why use functions? 🐸
    - **Reusability**: prevents you from repeating code that you’ve written before
    - **Algorithms**: helps to create or formulate algorithms
    - **Clean Code**: organizes a solution into a function
    - **Single Serving**: a block of code that solves a single problem
 
### Strings
	- a data type that is a sequence of characters
	- rep ALL character/symbol based data type in Python 3
	- use single/ double quotations to denote strings
	- Variables can hold string type values 
	- can have empty strings 
	- can create string with a space 
	- Strings are comparable; therefore can create boolean expressions that compare strings
	
#### Comparing strings
	- When a string is sorted/compared, it follows the ASCII order.
	- Numeric Symbols are **less** than uppercase characters
	- Uppercase characters are When a string is sorted/compared, it follows the ASCII order.
numeric < uppercase<lowercase

#### Indexing
	- Examine: word = “Hello”
	- print(word[2]) # outputs → ‘l’
	- print(word[0]) # outputs → ‘H’
	- print(word[-1]) # outputs → ‘o’
	- print(word[5]) # index error

#### Slicing 🐸
	- In Python, we can create a new subset of a sequence if the data-type is slicable.
		-  we can create new version that is a subset of an original string.
	- word = “Hello”
		print(word[1:3]) → ‘el’
		print(word[-1:-3:-1]) → ‘ol’ 
		print(word[0:5:2]) → ‘Hlo’
		print(word[2:2]) → ‘’ # empty string
		print(word[6:2]) → ‘’ # empty string
		**print(word[:]) → ‘Hello’
		print(word[::-1]) → ‘olleH’
		print(word[::-2]) → ‘olH’**
#### Immutability 
	- Despite the fact that we can index and slice strings, **Strings are immutable**.
		- immutability -->  Where the data type value can’t be altered without recreation.
Example:
name = “Jim”
name[0] = “T” #Will produce an error 
Integer, Floats, Boolean, and Strings are all Immutable

#### String operations
a="Hi" b='bye'
concatenation --> a+b--> 'Hibye'
repetition --> a*2 --> 'HiHi'

### Lists
	- collection of data item values
	- Each item can be same or different data type (Int, Float, String, Boolean, List)
	- Each items are separated by a comma except the last
	- A list is denoted by square brackets
	- A list is iterable; therefore, we can traverse through it with a for loop
	- ** lists are indexable and sliceable **
	- **lists are MUTABLE **
#### List methods 
	- .append(item) will add the argument: item to the end of the list. Append only adds one item at a time
	
	- .extend(another_list) allows us to combine two lists together into one list … the argument of .extend() has to be a list
	
	- .insert(location, item) allows us to add an item at a specific location in a list  🐸
		- If the location is beyond the size, it will add it to the end
		- location can be negative
		- If the location already has a value, it will shift everything at the location onwards to the right to add the item
	
	- .pop(target_index) will remove a value located at the target_index and RETURN THE VALUE
	
	-  .remove(target_value) will remove the first occurance of the target value if it exists in the list.
		- If the target_value doesn’t exist, it will produce an error
			- we CANNOT use .remove in a for loop to remove values 
					  eg: 
						array=[a,b,b,a]
						for i in array:
							if i == 'a':
								array.remove(i)
			- so here, in a for loop, eachg value is only checked over once, if we tell program to remove value at index of [2], after it is done
			  every item position will shiftt up by one ( each index valye is shifted to the left)
			- so, in the for loop logic it already checked the value at index of 2, it does NOT recogize that since the array items shifted up by 
			  one in the list that there is NOW a new item at the index of 2 WHICH the program DID NOT CHECK
			- regardless, it skips it and moves on to checking the index of 3 value 
					- if we want to remove values from an array, USE WHILE LOOP
						- set condition: while 'a' in array: ....
							- therefore each value in the array wil be checked MORE than once WHICH ensures no value is skipped 
							
**List Additions works the same as the extend() function, but it creates a new list.**
**(append, extend, insert MUTATES a list … list addition creates new list)**  🐸

