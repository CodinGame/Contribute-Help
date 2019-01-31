@TODO

# General Guidelines <a name="guidelines"/>

When creating your game, we suggest you follow these guidelines in order to improve both its performance and players experience.

- Viewer
  - The viewer must be self-explanatory. _A player should understand most of the rules from a replay_
  - The viewer must contain the avatars and nicknames of current players (if multi).
- Referee
  - The referee must end a player's program when receiving an unrecognizable command.
  - The referee must send an error message in the console when receiving an invalid but recognized command.
  - The referee must stop the game early if the game is stale or already decided.
  - The referee must not crash. All exceptions must be caught (especially during the parsing of a Player’s actions, where most errors occur).
  - Indices must start at 0, not 1. The origin is always the top left pixel/tile.
The game should also respect the [statement guidelines](pages/technical/statement.md#guidelines)

# Best Practices

- Protocol/Stub
  - If options for a player are limited, they should be sent in input (ex: [Wondev Woman](https://www.codingame.com/ide/puzzle/wondev-woman))
  - The player's id should be 0.
  - The player's input should be sent first in loops.
  - Any non-explicit variable should be explained with a comment.
  - The stub should not change between leagues.
  - The generated stub should not contain more than 45 lines in Java.
  - The number of variables per loop should not exceed 10.
  - There should be maximum 2 loops.
- Gameplay
  - The game should be turn-based. Only perform checks (collision, presence, etc.) at the end of a turn.
  - The total entities should not exceed 200.
  - The maximum number of rounds should not exceed 250.
  - The maximum alloted time per player should not exceed 25 seconds.
- Graphics
  - Privilege the use of Sprites over Shapes (Rectangle, Circle, etc.)
  - Less than 2Mb in total should be used.
  - The minimum font size should be 36px.
  - The choice of colors should take into account color-blind people as much as possible.
  - .png and .jpg assets should be minified.
- [Statement](pages/technical/statement.md#game-statement)