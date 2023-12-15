import random

def guess_the_number():
    secret_number = random.randint(1, 100)
    
    print("Welcome to Guess the Number Game!")

    while True:
        guess = int(input("Enter your guess: "))

        if guess < secret_number:
            print("Too low! Try again.")
        elif guess > secret_number:
            print("Too high! Try again.")
        else:
            print("Congratulations! You guessed the number.")
            break

if __name__ == "__main__":
    guess_the_number()
