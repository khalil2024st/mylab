# mylab
import random

print("Welcome to the Guessing Game!")
print("I'm thinking of a number between 1 and 25.")
secret_number = random.randint(1, 25)
user_guess = None
while user_guess != secret_number:
    user_guess = int(input("Please enter your guess: "))
    if user_guess < secret_number:
        print("Too low! Try again.")
    elif user_guess > secret_number:
        print("Too high! Try again.")
    else:
        print(f"Congratulations! You've guessed the number {secret_number} correctly!")
