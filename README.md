# FreeCodeCampPythonCourse

Hi All! This repository was created to document my learnings and projects from FreeCodeCamp's Python course offered via YouTube. If you're interested in learning more about the course please visit https://www.youtube.com/watch?v=rfscVS0vtbw

## Set Up
*I used a windows computer to complete this course*
1. Download Python 3 https://www.python.org/downloads/
2. Download a text editor, I'll be using PyCharm https://www.python.org/downloads/
3. Create a new python project called app.py

## Hello World
The most introductory program is Hello World!, to create it write the following command:
```
print("Hello World!")
```
Now click Run to produce the message on the console

## Drawing a Shape
To draw an isolceles triangle, write the following command
```
print("   /|")
print("  / |")
print(" /  |")
print("/___|")
```
When it comes to Python, the lines of code are read in order from top to bottom

## Variables & Data Types
A variable is essentially a container that stores data values, these facilitate managing data within programs
```
print("There once was a man named George,")
print("he was 70 years old.")
print("He really liked the name George.")
print("but didn't like being 70.")
```
If you write in the above command & then run it, you'll produce the story of George. Now imagine, that the story was hundreds of lines of code and you had decided to change the main character's name & age. Instead of going line by line and changing those fields, you could utilize a variable to store those new field values and then use the variable to mass edit the story. 

To create a variable for the man's name you'll need a variable, an assignment operator, and a value. In this case the variable will be character_name, it's important to use underscores in place of spaces in variable names. As for the assignment operator, you'll need to use an equals sign. Lastly, the varibale here will be the man's new name, John. 
```
character_name = "John"
```
Now create another variable to change the character's name
```
character_age = "35"
```
In order for these variables to be connected to the story, within the story you'll need to have referred to the appropriate variables as seen below

```
character_name = "John"
character_age = "35"

print("There once was a man named " + character_name + ", ")
print("he was " + character_age + " years old. ")
print("He really liked the name " + character_name + ". ")
print("but didn't like being " + character_age + ".")
```
To keep text unchanged surround it using quotation marks, to add the variable utilize a plus sign.
Additionally, if you wanted to change the character's name half way through the story you could insert the name variable as an additional line at the point where the name change should occur. Remember Python is read from top to bottom, so it will take the updated variable and change the data for the lines that follow 
```
character_name = "John"
character_age = "35"

print("There once was a man named " + character_name + ", ")
print("he was " + character_age + " years old. ")

character_name = "Mike"
print("He really liked the name " + character_name + ". ")
print("but didn't like being " + character_age + ".")
```
## Storing data within a variable using strings, numbers, and booleans
Strings: Used for texts, numbers, etc. must use quotation marks 
```
character_name = "George"
```
Number: Uses an integer
```
character_age = 50
```
Booleans: True or false values are stored here
```
isRed = True
```
## Working with Strings
Remember strings belong inside quotation marks 
```
print("Hello World!")
```
Now in order to create a new line you need to add a "\n" where you want the new line to begin
```
print("Hello\nWorld!")
```
If you want to include a quotation mark use "\""
```
print("Hello\"World!\"")
```
You can use variables within strings as well in order to facilitate future changes and to concatenate strings. The variable phrase will be used in this example
```
phrase = "Giraffe Academy"
print(phrase)
print(phrase + " is cool.")
```
Functions perform specific operations, for example modify strings or obtain information about the strings. The following functions change the text to lower and upper case
```
phrase = "Giraffe Academy"
print(phrase.lower())
print(phrase.upper())
```
If you wanted to find out if the string was in uppercase, you could use the following function that will return a true or false reponse
```
phrase = "Giraffe Academy"
print(phrase.isupper())
 ```
 Combining functions is also possible. For example you could convert the text to uppercase and check whether it is or is not in uppercase using the same line of code
 ```
 phrase = "Giraffe Academy"
 print(phrase.upper().isupper())
 ```
 To find the number of characters within a string use len
 ```
phrase = "Giraffe Academy"
print(len(phrase))
 ```
 In python, strings get indexed from the number 0. So if you wanted to find out the first character in a string you would use the following function
 ```
phrase = "Giraffe Academy"
print(phrase[0])
```
The index functions can tell you where a specific character is located within a string. A value that you give to a function is a parameter. 
```
phrase = "Giraffe Academy"
print(phrase.index("a"))
```
The replace function allows you to replace portions of a string. This example uses two parameters, the first is the text that you want to replace, the second is the text that should replace the the first.
```
phrase = "Giraffe Academy"
print(phrase.replace("Giraffe","Elephant"))
```
## Working with Numbers
When it comes to working with numbers in Python, you'll be able to run arithetic. Decimals and negatives are accepted. The following line returns the number 5
```
print(1 + 4)
```
Order of operations is followed in Python, the first line returns 17, while the second returns 27 due to the parenthesis
```
print(3 * 4 + 5)
print(3 * (4 + 5)) 
```
Modulus operator helps determine the remainder when it comes to division. The following line will return 1, since it's the remainder of 10 divided by 3. 
```
print(10 % 3)
```
You can also use variable to store numbers
```
my_num = 5
print(my_num)
```
Aside from basic arithmetic, you can also convert numbers to strings in the event that you wanted to print the number next to text. The following number would return, "5 is my favorite number"
```
my_num = 5
print(str(my_num) + " is my favorite number")
```
Math functions can give you information about numbers or perform operations. 
The ABS function gives you the absolute number of a value. The following retunrs 5 
```
my_num = -5
print(abs(my_num))
```
The POW function allows numbers to have an exponent. This functions requires two numbers, one as a base and the other is the power. The following returns 9 
```
print(pow(3, 2))
```
The Max and Min functions can help you determine which number is either the largest or smallest. The following returns 6 for the first line and 4 for the second.  
```
print(max(6, 4)) 
print(min(6, 4))  
```
Additionally, Python allows you to round numbers by using "round". The following returns 3. 
```
print(round(3.3))
```
You can obtain additional functions through Python's library using the following line
```
from math import *
```
Some of those functions include floor and ceil which rounds the number down or up. the following returns 3 for the first line and 4 for the second. 
```
from math import * 
print(floor(3.7))
print(ceil(3.7))  
```
To find the square root of a number, use  SQRT. The following line  returns 4. 
```
from math import * 
print(sqrt(16))
```
## Getting Input From Users
Allow user to input info into our program, we then store the info in a variable that will be used later.

For example, the first two lines below are the variable that will hold the user's information, the third line will return Hello (user's name)! You are (age)
```
name = input("Enter your name: ")
age = input("Enter your age: ")
print("Hello " + name + "! You are " + age)
```
## Building a Basic Calculator
This project will request two numbers from the user, those will be stored in two separate variables, 
```
num1 = input("Enter a number: ")
num2 = input("Enter another number: ")
result = int(num1) + int(num2)
print(result)
```
If you use the code above, it'll only work w/ whole numbers. The first two lines are the variables that store the user's information, the third adds them, and the fourth prints. In order to add decimal numbers, use float as seen below
```
num1 = input("Enter a number: ")
num2 = input("Enter another number: ")
result = float(num1) + float(num2)
print(result)
```
## Mad Libs Game
The Mad Libs Game will request information from the user and store those into variables that will then be printed 
```
color = input("Enter a color:")
plural_noun = input("Enter a plural noun:")
celebrity = input("Enter a celebrity's name:")

print("Roses are " +color)
print (plural_noun + " are blue")
print("I love " + celebrity)
```
## Lists
Lists help manage large amounts of data within Python. Typically related values are entered in lists. Within lists you can store strings, numbers, etc. 
Index is the position of the elements within the list, the count starts at 0. This is useful for printing a specific element ex: the following will print the first element which is Kevin's name.
```
friends = ["Kevin", "Karen", "Jim"]

print (friends[0])
```
If you use negatives, you would start from the right side, those numbers begin at -1. Ex: the following will print Jim
```
friends = ["Kevin", "Karen", "Jim"]

print (friends[-1])
```
If you wanted to print all the elements after a certain index, you could write the number followed by a colon. For example, the following will produce all names after index 1, including itself.
```
friends = ["Kevin", "Karen", "Jim"]

print (friends[1:])
```
If you needed a range, then you would enter the index that the list should begin on and the number after the last index you want included. Ex: the following will print, Karen and Jim's names, but not any after. 
```
friends = ["Kevin", "Karen", "Jim","Oscar","Toby"]

print (friends[1:3])
```
If you needed to modify a value inside an arrray, you could by adding a line that has the variable and new value
```
friends = ["Kevin", "Karen", "Jim","Oscar","Toby"]
friends[1] = "Mike"
print (friends[1:3])
```
## List Functions
Extend function allows you to take a list & append another one to it
```
lucky_numbers = [4, 8, 15, 16, 23, 42]
friends = ["Kevin", "Karen", "Jim", "Oscar", "Toby"]
friends.extend(lucky_numbers)

print (friends)
```
You can use the append function to insert additional elements to an existing list, however, this will always add the new items to the end of the list
```
friends = ["Kevin", "Karen", "Jim", "Oscar", "Toby"]
friends.append("Jerry")

print (friends)
```
If you want to add an element at a specific point, you would use the insert function. For this you will need two parameters, the first is the position, then the name of the element
```
friends = ["Kevin", "Karen", "Jim", "Oscar", "Toby"]
friends.insert(1, "Kim")

print (friends)
```
Use the remove funciton to remove an element from the list
```
friends = ["Kevin", "Karen", "Jim", "Oscar", "Toby"]
friends.remove("Jim")

print (friends)
```
You could also use the clear function to remove all elements within a list
```
friends = ["Kevin", "Karen", "Jim", "Oscar", "Toby"]
friends.clear()

print (friends)
```
The pop function can be used to remove the last element from a list
```
friends = ["Kevin", "Karen", "Jim", "Oscar", "Toby"]
friends.pop()

print (friends)
```
If you needed to know if a certain element was in a list use the index function within the print function, it'll also give you their index position
```
friends = ["Kevin", "Karen", "Jim", "Oscar", "Toby"]

print (friends.index("Oscar"))
```
You could also count how many times an element appears within a list, in this example there are two Jims
```
friends = ["Kevin", "Karen", "Jim", "Oscar", "Toby", "Jim"]

print (friends.count("Jim"))
```
You could also sort the list Alphabetically or numerically (if you entered in integers) by using the sort function
```
friends = ["Kevin", "Karen", "Jim", "Oscar", "Toby", "Jim"]
friends.sort()
print (friends)
```
to Reverse the order, use the reverse function
```
friends = ["kevin", "Karen", "Jim", "Oscar", "Toby", "Jim"]
friends.reverse()
print (friends)
```
If you wanted to make a copy of the currrent list use the copy function
```
friends = ["kevin", "Karen", "Jim", "Oscar", "Toby", "Jim"]
friends2 = friends.copy()
print (friends2)
```
## Tupples
Tupples can store data, similiar to a list. Except they can't be changed, deleted, etc. Use the following to create a tupple for x, y coordinates
```
coordinates = (4, 5)
print(coordinates[0])
```
## Functions
Are a collection of code that perform a specific task
The code within a function will only perform when we add a calling. Here the second   
sayhi() serves as the calling
```
def sayhi():
    print("Hello User")
sayhi()
```
name all functions in lowercase, if multiple words use an underscore to separate the words in the name. The following function is an example of the ability to utilize Python to produce requested commands through functions. 
```
def say_hi(name, age):
    print("Hello " + name + ", you are " + str(age))

say_hi("Mike", "35")
say_hi("Steve", "80")
```
