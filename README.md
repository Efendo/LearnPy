# LearnPy
This is a website to learn programming in Python.
## Download Python
get the interpreter from the [Official Python Website](https://www.python.org/)

## What Code editor to use
the editor use want to use is your Choice but here is a list of some recommended ones:
1. VSCode: VSCode is a lightweight editor for alot of languages
2. PyCharm IDE: PyCharm is a dedicated Python IDE
4. Emacs: a terminal application that feels like an entire OS
5. Neovim / Vim: A powerfull text editor
6. Nano / Pico: Another powerfull text editor
7. IntelliJ IDEA: with the python plugin its a good python IDE

## The basics
the first thing ill teach you is print(). in python yoou dont need ; {} pyython use indentation istead of {} so yes indentation matters in Python.
heres how to use print:
````
print("Hello, Python!") # in programming "" or '' specifies that the data is a string
````

### Variables
Variables are really importent in programming. They store data.
in most programming languages you have to specify the type of a Variable, in python it auto detects the variable type
heres an example:

Java:
````
String Demo = "this is a demo";
````

Python:
````
Demo = "this is a demo"
````

heres all variable types:
int | full number
float | Floating point numbers
complex | complex numbers
bool | boolean
String | text
io.TextIOWrapper | Files

### Loops and Conditions
Loops and Conditions are an importent part in programming

'if' only does an action if the condition returns true or 1
example:
````
if condition:
    action
````

'for' loops do stuff the specified amount of time:
example:
````
for i in range(0, 11):
    print(i)
# output: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10
````

'while' loops do something while a condition is true:
example:

````
while(true):
    print("this is a")
    print("While loop")
# Ofcourse it runs for ever because the condition is always true
````

## getting input
to get input in python use the 'input()' method
example:
````
prompt = input("type something: ")
print(prompt)
````

## functions
using functions shortens your code alot. to define one type 'def function(input)'
heres an example:
````
def printX3(text):
    print(text * 3)
````

## example 1: even or odd number checker
````
def check(num):
    if num % 2 == 0:
        return "even"
    else:
        return "uneven"

print(check(int(input("enter a number: "))))
````

## example 2: quiz game
````
points = 0

def question(question, AAnswer, BAnswer, APoints, BPoints):
    print(question)
    print("--------------")
    print("A: " + AAnswer)
    print("B: " + BAnswer)
    answer = ""
    answer = input("answer: ")
    if answer == "a":
        return APoints
    else:
        if answer == "b":
            return BPoints

points = points + question("who invented python", "Guido van rossum", "dennis richie", 1, 0)
points = points + question("What is faster", "Python", "Java", 0, 1)
# add more questions if you want
print("you got: " + str(points))
````
