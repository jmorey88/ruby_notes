# ** Learn to Program**
## **Intro**

- coding is telling a computer how to do something using a language
- Ruby is a good starting language to learn because it is simple and user friendly
- code is not built is is grown and should be made to be flexible to changes
- dont repeat yourself “DRY”
- always code things as simply as possible

## **Chapter 1 Getting Started**

- text editors are used for write the program
- Ruby interpreter runs your program
- command line tells computer which programs to run
- always make sure you choose good text editor 

### **1.1 Windows**

- first install Ruby from http://rubyinstaller.org/ and download highest version
- make folder and desktop for files
- get text editor Notepad++ is recommended  http://notepad-plus-plus.org/
- access command line start menu, select accessories, then command prompt
- from here you can access inside of computer 
- cd, or change directory will let you call on your different files and get info about them

### **1.2 Mac OS X**

- ruby should already be installed on Mac
- good test editor is TextMate http://macromates.com/ but it costs
- TextWrangler is a good free one Http://www.barebones.com/products/textwrangler/
- make a program folder on desktop
- finder, to applications/utilities and open
- your last log in should be displayed
- this is where you access different folders and files in your computer

### **1.3 Linux**

- install Ruby 
- choose text editor
- create directory for files

## **Chapter 2 Numbers**

- first program 
- puts 1 + 2….3 will be returned
- save program as calc.rb, and run by typing ruby calc.rb into command line 
- 3 will print on screen

### **2.1 Did it Work**

- make sure your run program properly from command line

### **2.2 Introduction to Puts**
 
- **puts** puts what you type on the screen

### **2.3 Integer and Floats**

- in most comp languages **integers** are numbers without decimal points and **floats** are numbers with decimal points
- floats are not often used since most computer outputs are not in partial numbers like emails or messages

### **2.4 Simple Arithmetic**

- “+” “-“ “*” “/“ are all used as basic math functions in Ruby
- If using integers only whole numbers will be returned…rounding down if needed

## **Chapter 3 Letters**

- groups of letters are called **strings**
- strings can be multiple words with punctuation, or they can be empty as long as they are between quotation marks

### **3.1 String Arithmetic**

- strings can be added together, just make sure you accommodate for spaces if need be
- and strings can be multiplied if they need to be repeated multiple times

### **12 vvs. ’12’**

- 12 is a number and “12” is a string of two digits
- 12 + 12 = 24
- “12” + “12” = 1212
- “12 + 12” = 12 + 12

- 2 * 5 = 10
- “2” * 5 = 22222
- “2 * 5” = 2 * 5

### **3.3 Problems**

- “12” + 12, or “2” * “5” don’t work because multiplying words or adding words to numbers doesn’t work
- you could write “pig” * 5 but not 5 * “pig”
- pig 5 times can be printed, but 5 can’t be printed “pig” times
- puts “You’re swell!” Will not work because ruby cannot tell differ between from apostrophe and single quote
- instead put “you/‘re swell!”
- backslashes are used as escape between to characters, and sometimes translated to apostrophe
- “you\’re swell!” = You’re swell!
- “backslash at the end of a string: \\” = backslash at the end of a string: \
- “up\\down” = up\down
- “up\down” = up\down  

## **Chapter 4 Variables and Assignment**

- so that a string a number can be used again a place for it to be stored is can be created
- you can create a variable and assign it whatever number or string you want
- variables can be insterted into or added to other strings
- varibales can be changed mid program 
- varibales can be switched back and forth between integer and string

## **Chapter 5 Mixing It Up**

- an integer and a string can not be added together so one must be changed

### **5.1 Conversions**

- to convert a variable you add .to_ + the letter indicating what you want to convert it to
- .to_s goes to a string, .to_i goes to an integer, .to_g goes to float
- if a string converting to an integer starts with a number that number will be turned to an integer
- if it starts with a letter it will convert to 0

### **5.2 Another Look at puts**

- puts litterally meants to put string
- so whenever you puts something it will convert it to a string first

### **5.3 The gets Method**

- gets is for get string
- when you put gets ruby will wait for the user to type something and press enter

### **5.4 Did it Work?**

- make sure you're running things through command line or there will be problems with gets

### **5.5 The chomp Method**

- when info is recieved from user using gets the enter at the end is saved as well
- to get rid of the enter so ruby doesnt print things funny you use .chomp
- variable.chomp cuts of the enter at the end and wont skip to a new line

### **5.6 A Few Things to Try

- write a program that asks for a name and returns nice to meet you + name
- write a program that asks for a number and then suggests a better number + 1

### **5.7 Mind Your Variables**

- when creating varibales always keep in mind what they are pointing to, integer, string
- always name your variables clearly so you remember what they are assigned to and why
- most common problems in programs come from not converting properly 

## **Chapter 6 More About Methods**

- **method** is what is done to an object.
- like a verb to a noun
- all methods must be attached to a noun
- not always by a dot

### **6.1 Fancy String Method**

- string methods are methods used on strings
- .reverse will reverse a string without changing the original string
- .length will return the number of characters in a string including the spaces
- .length returns and integer, so remember to return it to a string if thats how you want it printed
- .upcase changes all characters in string to uppercase
- .downcase changes all characters to lowercase
- .swapcase swithces uppercase to lower and vis versa
- .capitalize will upper case only the first letter of the string if its a letter
- .center will center your string with spaces on both sides, but you have to tell the method how many space
- .ljust and .rjust will pad the string on the left or right with spaces, however many you tell it

### **6.2 A Few Things to Try**

- create angry boss program that yells at you and fires you when you say something
- create a table of contents with specific spacing

### **6.3 Higher Math**

- high math problems are methods on numbers

### **6.4 More Arithmetic**

- "**" with give you the exponentiation 
- % gives you the remainder after the devision
- .abs will give you the absolute number

### **6.3 Random Numbers**

- rand will give you a ruby generated random number
- rand by itself will give you a number equal to or greater than 0 but less than 1
- rand(x) will give you a number greater or equal to zero and less than x
- srand or seed rand will let you set up a sequence of random numbers that can be replayed

### **6.4 The Math Object**

- Math objects are things usually found on a scientific calcualter, but in Ruby

## **Chapter 7 Flow Control**

- programs need to do more than just say things, they need to do things to

### **7.1 Comparison Methods**

- <, >, ==, <=, >=, != can all be used to determine if something is true or false
- usually when camparing you think integers, but strings can be compared too
- when comparing strings ruby looks at them alphabeticly
- is cat < dog yes it is true because cat is first alphebeticly 
- ruby also reads capital letters as less then lowercase
- so always downcase or upcase before you compare strings
- also make sure numbers are integers not strings, if they are rember 10 will read less then 2

### **7.2 Branching**

- branching is asking the program to do something if a certain criterea is met
- if x == y then do __ else do __
- branches can have branches but remember to always put end after any if statements started
- by setting up you variables if else and end with #notes inbetween, you can get a good idea of what blocks or tasks you need to ask your program to do

### **7.3 Looping**

- while statements allow you to make a program repeat a task until you want it to stop
- while x == y do __
- always make sure you have a way to end your loops or the program will get stuck in a loop and crash
- ctr c will get you out of a stuck loop if that ever happens

### **7.4 A Little bit of Logic**

- you can use elsif after if you want to continue adding new criterea 
- other operators used are && for and || for or ! for not
- these will help you get your program to conicesly run through multiple tests with minimal code

### **7.5 A Few Things to Try**

- write program printing out lyrics to 99 bottles of beer on the wall
- write program that ask for start year and end year and returns all leap years between

## **Chapter 8 Arrays and Iterators**

- an array is like a list of variables made on your computer
- they allow you to store data, and access it when you need it
- an array can include strings integers and other arrays
- and arrays index allways starts counting at zero
- each index in an array can be assigned a variale and reasigned
  
### **8.1 The Method each**

- .each allows you to do something with each variable in an array
- after you end an array with .each you must assign a variable to use for each index and put it in ||
- .each is like a loop but is a method
- methods like .each are called iterators
- iterators are allawys followed by a block which is telling ruby what to do with each variable

### **8.2 More Array Methods**

- some methods that worked on strings work on arrays too, like +, =, . length, or reverse
- you can .to_s an array to make it clear your working with strings
- when you puts an array remeber it puts each item individualy from the array unless joined
- push and pop allow you to remove items from the end or the begining of an array changing its length
- .last will call on the last item of an array

