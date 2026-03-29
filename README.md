# My-first-python-code-
This is my very first self-written Python project! I wanted to create something engaging that helps other beginners understand the core logic of programming through a fun game. 
What’s inside:
 Concepts Used: Only Loops and Conditional Statements (if/else). 
Goal: To show how simple basics can build a fully functional, interactive game. 
CODE:




import random

def secret(t):
    # This line is now inside the function
    print("----Welcome to guess number challenge----")
    
    # The loop is now indented, so it belongs to the function
    while True:
        try:
            guess = int(input("Guess the number between 1 and 100: "))
            
            if guess == t:
                print("You got it! Congratulations")
                break
            elif guess < t:
                print("Go higher, You are close")
            else:
                print("Go lower, You can do it")
        except ValueError:
            print("Please enter a valid number!")

# These are separate lines at the very bottom (no indentation)
y = random.randint(1, 100)
secret(y)
