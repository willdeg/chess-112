# ♟️ Chess 112

A Java desktop chess game with local two-player matches and three levels of computer opponents. Originally built in **2020** by **William DeGroot, Will Fishell, and Arianna Mordy**.

This repository preserves the original project and commit history from [williamdegroot/Chess-112](https://github.com/williamdegroot/Chess-112), with refreshed documentation.

## Features

- A graphical board built with Java Swing.
- Local two-player games or a match against the computer.
- Easy, medium, and hard AI, with minimax search used by the medium and hard opponents.
- Move validation, check/checkmate and stalemate handling, and threefold-repetition notifications.
- Keyboard controls for castling and pawn promotion.

## Play

Install a Java Development Kit (JDK) that provides `javac` and `java`. From the repository root:

```bash
javac *.java
java Main
```

Keep `Instructions.txt` and the `src/` image folder in place, and launch from the repository root so the game can find them. Choose a human or computer opponent in the startup dialogs, then select an AI difficulty if applicable.

The original project uses only standard Java libraries. Medium and hard AI can take several seconds per move; the original README notes approximately 5–10 seconds.

## Controls

White moves first. Click a piece, then click its destination. Click another piece of your own to change your selection.

| Action | Control |
|---|---|
| Move a piece | Click the piece, then the destination square |
| Promote a pawn | Immediately press `q`, `r`, `b`, or `k` for queen, rook, bishop, or knight |
| Castle kingside | `d` |
| Castle queenside | `a` |

See [the original instructions](Instructions.txt) for the game's detailed rules and prompts.

## Code map

- `Main.java` — application window, setup dialogs, and input handling.
- `Board.java`, `Square.java`, `Team.java` — board state and teams.
- `Piece.java` and the individual piece classes — movement logic.
- `Computer.java`, `EasyComputer.java`, `MediumComputer.java`, `HardComputer.java`, `MiniMax.java` — computer opponents and search.
- `src/` — chess-piece images.

## Credits

Created by **William DeGroot, Will Fishell, and Arianna Mordy**. The original [README.txt](README.txt) is retained alongside this updated overview. The 2026 documentation refresh does not change the game code.
