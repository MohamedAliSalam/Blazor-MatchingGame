# Memory Matching Game (Blazor WebAssembly)

A timed memory-matching game that runs in the browser. Flip two cards at a time, keep the pairs you match, and race the clock until the board is clear.

I built it to learn how component state works in Blazor WebAssembly: keeping the board, the flipped cards and the timer in one component, and re-rendering as they change.

## Features

- Shuffled grid of face-down cards
- Matched pairs stay face up; mismatches flip back after a short delay
- A stopwatch tracks how long the board takes to clear
- Congratulations message when every pair is found
- Reset button to start a new board at any time

## Run it locally

Requires the [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0).

```bash
git clone https://github.com/MohamedAliSalam/Blazor-MatchingGame.git
cd Blazor-MatchingGame
dotnet run
```

Then open the URL printed in the terminal.

## How it's built

| File | What it does |
|---|---|
| `Components/GameBoardComponent.razor` | All game logic and UI: shuffling, flipping, matching, the stopwatch and reset |
| `Pages/Index.razor` | Hosts the game board |
| `wwwroot/css/app.css` | Card and board styling |

## License

[MIT](LICENSE)
