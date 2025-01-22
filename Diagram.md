

```mermaid
flowchart TD
    A[Start] --> B[Generate a random number between min and max]
    B --> C[Prompt user for a guess]
    C --> D[Validate input]
    D -->|Invalid: Non-numeric or out of range| E[Display error message]
    E --> C
    D -->|Valid| F[Compare guess to random number]
    F -->|Guess < Random| G[Display "Too low"]
    G --> C
    F -->|Guess > Random| H[Display "Too high"]
    H --> C
    F -->|Guess == Random| I[Display "Correct!"]
    I --> J[End]
```