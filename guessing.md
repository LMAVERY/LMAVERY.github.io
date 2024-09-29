## Random Guessing Game Flowchart

```mermaid
flowchart TD
    Start([Start]) --> Generate[Generate Random Number]
    Generate --> Input[Get User Input]
    Input --> Check[Check User Input]
    Check -->|Valid| Compare[Compare Guess with Random Number]
    Check -->|Invalid| Input[Get User Input Again]
    
    Compare -->|Too High| Feedback1[Provide 'Too High' Feedback]
    Compare -->|Too Low| Feedback2[Provide 'Too Low' Feedback]
    Compare -->|Correct| Feedback3[Provide 'Correct' Feedback]
    
    Feedback1 --> Input
    Feedback2 --> Input
    Feedback3 --> End([End])

Step 4: Step Descriptions
Start: The beginning of the game.
Generate Random Number: The computer generates a random number within a specified range (e.g., 1 to 100).
Get User Input: The program prompts the user to enter their guess.
Check User Input: The program checks if the input is valid (numeric and within range).
If valid, it proceeds to compare.
If invalid, it prompts the user to enter the guess again.
Compare Guess with Random Number: The program compares the user's guess with the generated random number.
If the guess is too high, it provides feedback and prompts for another guess.
If the guess is too low, it does the same.
If the guess is correct, it provides a congratulatory message.
End: The game ends after a correct guess.


