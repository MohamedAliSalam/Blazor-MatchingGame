# Memory Matching Game Readme

## Overview
This is a simple Memory Matching Game implemented using Blzor Webassembly. The game presents a grid of cards face down, and the player's objective is to flip pairs of cards to find matching pairs.

## Features

- The game board consists of a grid of cards, each containing a hidden value.
- Cards can be flipped by clicking on them.
- If two flipped cards match, they remain visible.
- If two flipped cards do not match, they are flipped back after a brief delay.
- The game keeps track of the time taken to complete and displays it.
- Once all pairs are matched, a congratulatory message is displayed.
- Players can reset the game board at any time.

## How to Use

1. Clone or download the code repository.
2. Ensure you have the necessary development environment set up for C# with Razor syntax.
3. Run the application.
4. Click on cards to flip them and try to match pairs.
5. Continue until all pairs are matched or use the reset button to start a new game.

## Code Structure
- The main game logic is implemented in the `GameBoardComponent.razor` file.
- The `Card` class defines the properties of each card (e.g., value and whether it's flipped).
- The game board is initialized with a certain number of pairs of cards (defined by `TotalPairs`).
- Cards are shuffled randomly before the game starts.
- The `FlipCard` method handles the logic when a card is flipped.
- The `ResetGame` method initializes a new game.
- The stopwatch is used to track the time taken to complete the game.
- Razor syntax is used for UI rendering, including conditionally displaying messages and handling user interactions.

## Contributing

Contributions to the game are welcome! Feel free to fork the repository, make changes, and submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

