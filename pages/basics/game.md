Coding games are turn-based games; they're most of the times associated with a viewer. They're built with the CodinGame Game Engine (sdk). See the technical details in the [sdk documentation](https://www.codingame.com/playgrounds/25775/codingame-sdk-documentation).

In an "infinite" loop, the player(s) must read the entries from the Standard Input stream and send a response to the Standard Output stream to play the game.

Each iteration of the _while_ loop corresponds to a turn of the puzzle where your code must read input data in stdin and output a "move" in stdout.

## Solo Games

Like for In/Out puzzles, the player plays against the game and must pass all test cases to solve the puzzle.

_Example: [Power of Thor](https://www.codingame.com/training/easy/power-of-thor-episode-1)
Each turn, the player must output a direction for Thor to take to finally reach the light._

The game loop is actually not infinite: there is a maximum number of turns allowed to solve each puzzle. Once your program sends the expected output or reached the expected state, the referee program (on CodinGame side) will end the loop.

## Bot Programming Games
 
Bot programming games are multiplayer games with a game loop. There are no test cases to pass.

The goal is not to output a solution but to create a bot (an AI) capable of playing a game in the given environment. 

Participants play against themselves in matches of 2 to 4 players in an arena. Once players submit their code (AI) in the arena, the system matches them against other players of the arena. Each match between players impacts their score, hence their ranking.

In each league but the last (Legend), there is a reference bot: the boss. Any player who ends up above the boss' score after their ranking battles are finished will be promoted to the league above.

Here's a [guide to get started in bot programming games](https://www.codingame.com/playgrounds/53785/tutorial-for-bot-programming-on-codingame). It's actually simpler than it looks!

## Optimization Games

Optimization games are games for which a player's score is computed based on specific criteria. All players are ranked against this score.

### StdIn/StdOut synch

It's really important to continue reading all input data on the stdin each turn; else, your program will desynchronize from the referee program.

With the same idea, if you start reading the input data of turn n+1 on the stdin without having sent a response in the stdout at turn n, the referee program will consider that your program did not respond in due time (timeout).