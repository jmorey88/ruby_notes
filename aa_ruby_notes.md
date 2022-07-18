# **Intro to Programming**

## **What is Programming**

- telling your computer to do something in the simplest way possible
- computer language is used to communicate commands to your computer

## **First Ruby Programs: Numbers and Strings**

- **puts** is most basic Ruby command telling Ruby to print a string
- **string** is a sequence of characters
- puts can also print numbers
- **integers** are what Ruby calls whole numbers
- **floats** are numbers with decimal points
- dont use commas when printing numbers 1000 or lager, ruby can read them
- Ruby uses traditional math operations
	-  “+” for plus
	- “-“ for subtraction
	- “*” for multiplication
	- “/“ for devision
- when dividing two numbers ruby will always round down, unless a float is given in the problem or **fdiv** is used
	‘puts(9.fdiv(2))
- “%” is called **modulo** and its functions is to return the remainder left after dividing two numbers

## **Variables**

- a **variable** is a place created in Ruby to store data
- variable names can contain letters or numbers but first character needs to be lowercase letter
- if variable name has multiple words they need to be separated with a _ not a space
- because it is a variable it can always be reassigned later in the program

## **User Input**

- **gets** is a method used to prompt a user for input
- user input allows programs to do different things

## **Methods with no Arguments**

- gets is a method that doesn’t take an argument.
- you don’t need to put parentheses at the end
- parentheses are left out to make coding look cleaner

## **Converting Between Strings and Integers**

- **to_i** is a method used to convert a string to an integer
- **to_s** is a method used to convert an integer to a string
- this is useful when needing to convert user input for the program to understand
- if a user inputs numbers as a string they need to be converted to integers for Ruby to understand them as numbers and not words

## **The *chomp* Method**

- when a string is entered by a user it Ruby reads the return command the user pressed to send the string
- when the string is later printed by the program, Ruby will print the string with the return command starting a new line.
- **gets.chomp** is a method that will remove any return command at the end of a string.
- remember chomp produces a new string and does not adjust the existing string

## **What are Methods?**

- methods are like verbs in ruby and strings are the nouns
- when a method is called, it does something to one or more objects
- object.method, method is always on right of period

## **Comparisons**

- greater than or less than signs “<, >” are used to compare objects 
- Ruby will return True or False
- it is different from the strings “true” and “false”
- “==“ and “!+” are used as equal to and not equal to
- remember = assigns a variable, and == compares two objects

## **If, Else, and Elsif**

- code branching is what allows a program to different things depending on the conditions
- putting **if** allows the program to run a test and do something depending on the outcome of that test
- after “if”, first the test is written, and then the body telling it what to do.
- always remember to indent the body, and don’t forget to put end!
- you can add another branch of code by using **else**
- *if* the test is true do something *else* do something else
- if you want 3 or more branches you can use **elsif**
- *if* the test is true do something, *elsif* another test is true do something, *else* do something else

## **Logical Connectives**

- you can also ask Ruby to perform a task if multiple criteria are met with “&&” for and, “||” for or, and ! For negation 

## **Looping**

- using **while** can allow you to ask Ruby to continue running a test over and over until it meets the proper criteria 

## **Infinite Loops**

- If you don’t write a way out of a loop it will run infinitely and crash unless you press Ctrl key + C

## **Arrays**

- **arrays** are groups of data separated by commas stored in Ruby Programs 
- arrays are useful because different items in the array can be called on at different times,
- by giving each item a numerical value, the first item starting as 0, you can call and any or multiple items
- **.length** is a method for checking the length of an array

## **Adding or Removing From Arrays**

- **push** method is what allows you to add an item to the *beginning* of an array
- likewise, you can use **unshift** to add an item to the *end* of an array
- array.push, or array.unshift
- using **shift** and **pop** you can remove items from an array
- shift removes from the beginning and pop removes from the end

## **Setting Positions in an Array**

- just as you can call on any item in an array arr[idx], you can also set the item equal to something new
- arr[idx] = “something new”
- calling on an item beyond the array just puts a blank line

## **Strings Are Like Arrays**

- just like arrays strings are a collection of characters that have length and can be called on
- .length will give you the length of a string
- string[idx] will call on a specific character
- however, “abc” != [“a”, “b”, “c”]

## **Splitting a String; Joining an Array**

- putting **.split** after a string will break the sentence into an array of separate words
- putting **.join** after an array will turn the list of words into a string
- adding (“, “) a comma with a space will join the words with commas in-between 

## **Writing Your Own Methods**

- when you have code that needs to be repeated several times over in a program, writing your own method can come in handy
- def new_method(input) 
- and end the method
- everything between *def* and *end* is the body of the method
- the body only describes what will be done when that method is called
- a method is called by typing its name and adding input in parentheses 

## **Breaking Out of Loops**

- **break** will get you out of a loop.
- if you have a *while true* loop going, it won’t stop until otherwise prompted

## **Returning Early**

- by putting **return** you can stop a loop early or once it reaches a certain criteria