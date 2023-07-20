# Learning Python the Right Way: Program a Rock Paper Scissors Game in Python using PRIMM Approach

PRIMM is an approach that can help beginners master coding through structure lessons. 

## Contents
[Introduction](#Intro)

[Stage 1: Predict](#s1)

[Stage 2: Run](#s2)

[Stage 3: Investigate](#s3)

[Stage 4: Modify](#s4)

[Stage 5: Make](#s5)

## Meet PRIMM <a name="Intro"></a>

PRIMM stands for Predict– Run–Investigate–Modify–Make, representing the different stages of a lesson or series of lessons. It enables critical thinking about how programs work, and the use of starter programs to encourage the reading of code before writing it.

![Meet PRIMM](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/m76rdbvd1btkhp953384.png)

## Stage One: Predict <a name="s1"></a>
### The Structured Approach
Using the structured approach means that you need to breakdown each of the blocks of code and decide how they will work together. A structure chart is created to decide the hierarchy for the program.

![structure chart](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/amhj0ewdq4izmuv3kkhj.png)

It's time to concentrate on the function of the code after breaking it down using the structure chart.

## Stage Two: Run <a name="s2"></a>
Copy the lines of code provided below and paste it in your python IDE and run it.

```python
# import the extra functions 
from time import sleep
from random import randint

# set the game rules
rock = 1
paper = 2
scissors = 3

name = {rock: "Rock", paper: "Paper", scissors: "Scissors"}
rules = {rock: scissors, paper: rock, scissors: paper}

player_score = 0
computer_score = 0

# start game and return score
def start():
    print("Let's play Rock Paper Scissors")
    while game():
        pass
    return scores()

# the game func
def game():
    player = play()
    computer = randint(1, 3)              # let the computer randomly between 1 and 3
    outcome(player, computer)
    return restart()

# let the player play
def play():
    while True:
        print()
        player = input("Rock = 1\n Paper = 2\n Scissors = 3\n Kindly make a move: ")
        try:
            player = int(player)
            if player in [1, 2, 3]:
                return player
        except ValueError:
            pass
        print("Please choose between 1, 2 or 3")  

# the outcomes
def outcome(player, computer):
    print("1....")
    sleep(1)
    print("2....")
    sleep(1)
    print("3...")
    sleep(.5)
    print("Computer threw {0}!".format(name[computer]))  # string.format i.e use the computer choice to replace the {0}
    global player_score, computer_score
    if player == computer:
        print("It's a Tie!!")
    else:
        if rules[player] == computer:
            print("You're a genius")
            player_score += 1
        else:
            print("You're being lectured by a computer")
            computer_score += 1
    
# replay or restart func
def restart():
    decision = input("Will you like to play again? Y/N: ")
    if decision in ["Yes", "Y", "y", "yeah", "ofcourse"]:
        return decision
    else:
        print("See you next time")
        
# the score func
def scores():
    global player_score, computer_score
    print("Final_score")
    print("Player: ", player_score)
    print("Computer: ", computer_score)

if __name__ == "__main__":
    start()
```

### Check against predictions
Did everything go according to plan? Before proceeding to the next step, compare the code against all of the predictions.

## Stage Three: Investigate  <a name="s3"></a>

Trace each line of code and ensure that it functions as intended. You may explore how they function and learn more about the syntax by using [python cheat sheet](https://www.pythoncheatsheet.org). You can also use [trace table](https://www.101computing.net/using-trace-tables/) to trace the program and understand the conditions. Therefore, discuss each line of code and write a brief and concise comment about it.


## Stage Four: Modify <a name="s4"></a>
Modify code in small steps to add new functionality. You can start by renaming the variables and functions, tweaking the code and applying what has been learnt about the structure of the code. Moreover, you can gradually increase the difficulty accordingly.

## Stage Five: Make <a name="s5"></a>
Create a new but similar program to practice the programming skills that have been learnt. 

## Summary and Conclusion <a name="close"></a>
PRIMM is a way of structuring programming lessons that focuses on: 
1. Reading code before you write it
1. Working collaboratively to talk about programs
1. Reducing cognitive load by unpacking and understanding what code is doing
1. Gradually taking ownership of programs when ready

## References: 
THE PRIMM APPROACH: A scaffolded approach to structuring programming lessons.From: The Big Book of Computing Pedagogy

https://www.101computing.net/using-trace-tables/

BBC Bitesize Guides: Trace Table 
https://www.bbc.co.uk/bitesize/guides/z8n3d2p/revision/8

Structure Chart: https://press.rebus.community/programmingfundamentals/chapter/hierarchy-or-structure-chart/
