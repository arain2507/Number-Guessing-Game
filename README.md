# Number Guessing Game 🎯

A simple **Number Guessing Game** built using **Python**. The program generates a random number between 1 and 100, and the player has to guess the correct number with hints provided after each guess.

## Features ✅
- Random number generation (1-100)
- User input validation
- Provides hints (Too high / Too low)
- Tracks number of attempts
- Simple and interactive console-based game

## Installation & Usage 🚀
### **Prerequisites:**
- Python 3.x installed

### **Run the Game:**
1. Clone the repository or download the script.
2. Open a terminal or command prompt.
3. Navigate to the script directory.
4. Run the following command:
   ```sh
   python number_guessing_game.py
   ```
5. Follow the on-screen instructions to play the game!

## Code Overview 📝
```python
import random

def number_guessing_game():
    print("🎯 Welcome to the Number Guessing Game!")
    print("I have selected a number between 1 and 100. Can you guess it?")
    
    secret_number = random.randint(1, 100)
    attempts = 0

    while True:
        try:
            guess = int(input("Enter your guess: "))
            attempts += 1

            if guess < secret_number:
                print("🔼 Too low! Try again.")
            elif guess > secret_number:
                print("🔽 Too high! Try again.")
            else:
                print(f"🎉 Congratulations! You guessed the number in {attempts} attempts.")
                break
        except ValueError:
            print("⚠️ Please enter a valid number!")

if __name__ == "__main__":
    number_guessing_game()
```

## Future Enhancements 🌟
- Add difficulty levels (Easy, Medium, Hard)
- Implement a GUI version using Tkinter or PyQt
- Add a leaderboard to track top scores


## Contact 📩
For any queries or suggestions, feel free to reach out!


