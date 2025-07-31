import sys

valid_choices = ["rock", "paper", "scissors"]

player1 = input("Rock, paper, or scissors?").lower()
player2 = input("Rock, paper, or scissors?").lower()


def win (u1, u2):
    if(u1 == u2):
        return("Draw")
    elif(u1 == "rock"):
        if(u2 == "scissors"):
            print("Player 1 wins")
        else:
            print("Player 2 wins")
    elif(u1 == "paper"):
        if (u2 == "rock"):
            print("Player 1 wins")
        else:
            print("Player 2 wins")
    elif(u1 == "scissors"):
        if (u2 == "paper"):
            print("Player 1 wins")
        else:
            print("Player 2 wins")
    else:
        return("replay game")
        sys.exit()


win(player1, player2)
