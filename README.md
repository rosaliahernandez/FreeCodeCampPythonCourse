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
Now create another varible to change the character's name
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
To keep text unchanged surround it using quotation marks, to add the variable utilize a plus sign
