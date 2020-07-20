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
Coming Soon
