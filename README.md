# No1
Gameplay
```
import random

def guess_the_number():
    number_to_guess = random.randint(1, 100)
    guess = None
    attempts = 0

    print("Welcome to Guess the Number!")
    print("I'm thinking of a number between 1 and 100.")

    while guess != number_to_guess:
        try:
            guess = int(input("Take a guess: "))
            attempts += 1

            if guess < number_to_guess:
                print("Too low!")
            elif guess > number_to_guess:
                print("Too high!")
        except ValueError:
            print("Invalid input! Please enter a number.")

    print(f"Congratulations! You found the number in {attempts} attempts.")

if __name__ == "__main__":
    guess_the_number()
```
