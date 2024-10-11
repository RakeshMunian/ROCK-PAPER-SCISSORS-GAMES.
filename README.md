# ROCK-PAPER-SCISSORS-GAMES.
# ROCK,PAPER, SCISSORS GAMES.
import random
options = ("Rock", "Paper", "Scissors")
running = True
while running:
    player = None
    computer = random.choice(options)
    while player not in options:
        player = input ("Enter a choice (Rock, Paper, Scissors):")
    print (f"player :{player}")
    print (f"computer:{computer}")
    if player == computer:
        print ("It Is Tie!")
    elif player == "Rock" and computer =="Scissors":
        print ("You Win!")
    elif player == "Scissors" and computer == "Paper":
        print ("You Win!")
    elif player == "Paper" and computer == "Rock":
        print ("You Win!")
    else:
        print ("You Lose!")
    play_again= input ("play again?(y/n):").lower()
    if not play_again== "y":
        running= False
        print ("Thanks for Playing!")
