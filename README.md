# Number Guessing Game
## Overview
The Number Guessing Game is a simple console-based Java program where the player has to guess a number chosen randomly between 1 and 100. The player is allowed a limited number of trials to guess the correct number. If the player guesses correctly, they win; otherwise, they are informed whether the number is higher or lower than their guess, and they continue until they exhaust all trials.
## Features
- The game generates a random number between 1 and 100.
- The player has 5 trials (attempts) to guess the correct number.
- After each guess, the program informs the player whether the target number is higher or lower than their guess.
- If the player guesses correctly, the game congratulates them and ends.
- If the player does not guess the number within 5 trials, the game reveals the correct number.

## Program Flow
1. The program generates a random number between 1 and 100.
2. The player is allowed to make 5 guesses.
3. After each guess, the program provides feedback:
   - If the guess is correct, the game ends with a congratulatory message.
   - If the guess is incorrect, the program will indicate whether the target number is higher or lower than the guess.
4. If the player runs out of guesses, the program reveals the correct number.

## Compilation and Execution
### Requirements

- Java Development Kit (JDK) installed on your machine (Java 8 or above).
- An IDE or text editor for editing Java code (e.g., Eclipse, IntelliJ IDEA, or VS Code).
- Command Line/Terminal for compiling and running the program (optional if using an IDE).

### Steps to Compile and Run
1. Save the Java code in a file named `GFG.java`.
2. Open a terminal or command prompt.
3. Navigate to the directory where the `GFG.java` file is located.
4. Compile the Java file using the following command:
 bash
 javac GFG.java
5. Run the compiled program with the following command:
  bash
   java GFG
   ### Example Input/Output
   #### Input:
A number is chosen between 1 to 100. Guess the number within 5 trials.
Guess the number:
50
The number is greater than 50
Guess the number:
75
The number is less than 75
Guess the number:
63
The number is greater than 63
Guess the number:
70
The number is less than 70
Guess the number:
65
Congratulations! You guessed the number.

#### Output:
A number is chosen between 1 to 100. Guess the number within 5 trials.
Guess the number:
50
The number is greater than 50
Guess the number:
75
The number is less than 75
Guess the number:
63
The number is greater than 63
Guess the number:
70
The number is less than 70
Guess the number:
65
Congratulations! You guessed the number.

#### Input when the player exhausts all trials:

A number is chosen between 1 to 100. Guess the number within 5 trials.
Guess the number:
30
The number is greater than 30
Guess the number:
40
The number is greater than 40
Guess the number:
50
The number is greater than 50
Guess the number:
60
The number is less than 60
Guess the number:
55
You have exhausted K trials.
The number was 52.
```

#### Output:

```
A number is chosen between 1 to 100. Guess the number within 5 trials.
Guess the number:
30
The number is greater than 30
Guess the number:
40
The number is greater than 40
Guess the number:
50
The number is greater than 50
Guess the number:
60
The number is less than 60
Guess the number:
55
You have exhausted K trials.
The number was 52.
```

## Explanation of Code

### Key Functions:

- `guessingNumberGame()`: The main function that contains the logic for generating the random number, taking input from the user, and checking if the guess is correct. It also provides feedback about whether the guess is higher or lower than the target number.

- **Input Handling:** The program reads the user's input using the `Scanner` class and processes the guesses one by one.

- **Game Logic:** The game allows up to 5 trials. If the player guesses the correct number, the program prints a congratulatory message and ends. If the player exhausts all 5 trials, the correct number is revealed.

### Data Structures:

- **Variables:**
  - `number`: The randomly generated number that the player has to guess.
  - `K`: The maximum number of trials the player is allowed to make.
  - `guess`: The player's input on each trial.
  - `i`: A loop variable to iterate through the trials.

### Random Number Generation:

- The `Math.random()` method is used to generate a random floating-point number between 0 (inclusive) and 1 (exclusive). It is then scaled to a range between 1 and 100 by multiplying by 100 and adding 1, ensuring the number falls between 1 and 100.

## Limitations

- The program is limited to 5 trials, and there is no option to play more than once without restarting the program.
- The player must input guesses as integers. No other input validation is implemented for this program.

## Future Enhancements

- Allow the player to play multiple rounds without restarting the program.
- Provide an option to choose the difficulty level (e.g., number of trials or range of numbers).
- Implement input validation to ensure the player only enters valid integers.
  
## Conclusion

This Java program implements a simple number guessing game where the player has 5 attempts to guess a number chosen randomly between 1 and 100. The program provides feedback after each guess, and after 5 trials, it reveals the correct number if the player has not guessed it.

