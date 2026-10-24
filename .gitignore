import random

WORDS = [
    "python", "hangman", "computer", "keyboard", "programming",
    "challenge", "guitar", "garden", "library", "rocket",
    "planet", "jungle", "puzzle", "window", "forest"
]

def choose_word():
    return random.choice(WORDS)

def display_word(word, guessed_letters):
    result = ""
    for letter in word:
        if letter in guessed_letters:
            result += letter + " "
        else:
            result += "_ "
    return result.strip()

def hangman():
    word = choose_word()
    guessed_letters = set()
    wrong_guesses = 0
    max_wrong = 6

    print("Welcome to Hangman!")
    print("Guess the hidden word one letter at a time.")

    while wrong_guesses < max_wrong:
        print("\nWord: " + display_word(word, guessed_letters))
        print("Wrong guesses left:", max_wrong - wrong_guesses)

        guess = input("Enter a letter: ").lower()

        if len(guess) != 1 or not guess.isalpha():
            print("Please enter a single alphabet letter.")
            continue

        if guess in guessed_letters:
            print("You already guessed that letter!")
            continue

        guessed_letters.add(guess)

        if guess in word:
            print("Correct!")
        else:
            print("Wrong!")
            wrong_guesses += 1

        if all(letter in guessed_letters for letter in set(word)):
            print("\nYou win! The word was:", word)
            break

    else:
        print("\nYou lose! The word was:", word)

    replay = input("Do you want to play again? (y/n): ").lower()
    if replay == "y":
        hangman()
    else:
        print("Thanks for playing!")

if __name__ == "__main__":
    hangman()
