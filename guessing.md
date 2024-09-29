<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Guessing Game Flowchart</title>
    <script type="module">
        import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
        mermaid.initialize({ startOnLoad: true });
    </script>
    <style>
        /* Add some basic styling */
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        h1 {
            text-align: center;
        }
        .mermaid {
            text-align: center;
        }
    </style>
</head>
<body>
    <h1>Random Guessing Game Flowchart</h1>
    <div class="mermaid">
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
    </div>

    <h2>Step Descriptions</h2>
    <ol>
        <li><strong>Start:</strong> The beginning of the game.</li>
        <li><strong>Generate Random Number:</strong> The computer generates a random number within a specified range (e.g., 1 to 100).</li>
        <li><strong>Get User Input:</strong> The program prompts the user to enter their guess.</li>
        <li><strong>Check User Input:</strong> The program checks if the input is valid (numeric and within range).
            <ul>
                <li>If valid, it proceeds to compare.</li>
                <li>If invalid, it prompts the user to enter the guess again.</li>
            </ul>
        </li>
        <li><strong>Compare Guess with Random Number:</strong> The program compares the user's guess with the generated random number.
            <ul>
                <li>If the guess is too high, it provides feedback and prompts for another guess.</li>
                <li>If the guess is too low, it does the same.</li>
                <li>If the guess is correct, it provides a congratulatory message.</li>
            </ul>
        </li>
        <li><strong>End:</strong> The game ends after a correct guess.</li>
    </ol>
</body>
</html>

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


