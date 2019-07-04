Coding games are turn-based games; they're always associated with a viewer. They're built with the CodinGame Game Engine (sdk)., see the technical details in the [sdk documentation](https://www.codingame.com/playgrounds/25775/codingame-sdk-documentation).

In an "infinite" loop, the player(s) must read the entries in the standard input stream and send a response in the Standard Output stream to play the game.

There are three types of coding games.

**All coding games should**
- respect the [statement guidelines](pages/technical/statement.md#guidelines).
- respect the [games general guidelines](#guidelines).
- follow [best practices](#best-practice).

## Solo Puzzle (with a viewer)<a name="gameloop"/>

Like for In/Out puzzles, the player plays against the game and must pass all test cases to solve the puzzle.

_Example: [Power of Thor](https://www.codingame.com/training/easy/power-of-thor-episode-1)
Each turn, the player must output a direction for Thor to take to finally reach the light._

**Solo puzzles should also respect the [test cases guidelines](pages/technical/testcase.md#guidelines).**

[Learn how to create a Solo puzzle with the sdk](https://www.codingame.com/playgrounds/25775/codingame-sdk-documentation/create-a-solo-game)

## Multiplayer Game (bot programming) <a name="ai"/>

Participants play against themselves in matches of 2 to 4 players in an arena. No more test cases. Once players submit their code (AI) in the arena, the system matches them against other players of the arena. Each match between players impacts their score, hence their ranking.

In each league but the last (Legend), there is a reference bot: the boss. Any player who ends up above the boss' score after their ranking battles are finished will be promoted in the league above.

[Learn how to create a Bot Programming game with the sdk](https://www.codingame.com/playgrounds/25775/codingame-sdk-documentation/create-a-multiplayer-game)

## Optimization Puzzle <a name="opti"/>

Optimization puzzles are puzzles for which a player's score is computed. All players are then ranked against this score.

[Learn how to create an Optimization puzzle with the sdk](https://www.codingame.com/playgrounds/25775/codingame-sdk-documentation/create-a-multiplayer-game)

**Optimization puzzles should also respect the [test cases guidelines](pages/technical/testcase.md#guidelines).**

# General Guidelines <a name="guidelines"/>

When creating your coding game, we ask you to follow these guidelines in order to improve both its performance and players experience.

- **Graphics**
  - The graphics must be self-explanatory. _A player should understand most of the rules from a replay_
  - The graphics must contain the avatars and nicknames of current players (if bot programming).
- **Referee**
  - The referee must end a player's program when receiving an unrecognizable command.
  - The referee must send an error message in the console when receiving an invalid but recognized command.
  - The referee must stop the game early if the game is stale or already decided.
  - The referee must not crash. All exceptions must be caught (especially during the parsing of a Player’s actions, where most errors occur).
  - Indices must start at 0, not 1. The origin is always the top left pixel/tile.

# Best Practices <a name="best-practice"/>

When creating your coding game, we suggest you follow these best practices in order to improve both its performance and players experience.

- **Protocol/Stub**
  - If options for a player are limited, they should be sent in input (ex: [Wondev Woman](https://www.codingame.com/ide/puzzle/wondev-woman))
  - The player's id should be 0.
  - The player's input should be sent first in loops.
  - Any non-explicit variable should be explained with a comment.
  - The stub should not change between leagues.
  - The generated stub should not contain more than 45 lines in Java.
  - The number of variables per loop should not exceed 10.
  - There should be maximum 2 loops.
- **Gameplay**
  - The game should be turn-based. Only perform checks (collision, presence, etc.) at the end of a turn.
  - The total entities should not exceed 200.
  - The maximum number of rounds should not exceed 250.
  - The maximum alloted time per player should not exceed 25 seconds.
  - It's possible to write a working AI in a few minutes.
  - If several leagues exist: boss difficulty is low but requires knowledge of each new set of rules per league.
- **Graphics**
  - Privilege the use of Sprites over Shapes (Rectangle, Circle, etc.)
  - Less than 2Mb in total should be used.
  - The minimum font size should be 36px.
  - The choice of colors should take into account color-blind people as much as possible.
  - .png and .jpg assets should be minified.