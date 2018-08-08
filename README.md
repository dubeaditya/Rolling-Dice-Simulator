# Rolling-Dice-Simulator
I am making a DICE ROLLING SIMULATOR with the help of Python.

print("This is a Dice Rolling Screen")
import random

def roll(sides=6):
    num_rolled = random.randint(1,sides)
    return num_rolled

def main():
    sides = 6
    rolling = True
    while rolling:
        roll_again = input("Ready to roll? ENTER=ROLL . Q=QUIT. ")
        if roll_again.lower() != "q":
            num_rolled = roll(sides)
            print("You rolled a",num_rolled)
        else:
            rolling = False
    print("Thanka for playing.")

main()
