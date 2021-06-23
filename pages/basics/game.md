## Gameloop puzzles

Other puzzles contain an "infinite" while loop in the default code. It's the "game loop".

Each iteration of the while loop corresponds to a turn of the puzzle where your code must read input data in stdin and output a "move" in stdout.

The game loop is actually not infinite: there is a maximum number of turns allowed to solve each puzzle. Once your program sends the expected output or reached the expected state, the referee program (on CodinGame side) will end the loop.

It's really important to continue reading all input data on the stdin each turn; else, your program will desynchronize from the referee program.

With the same idea, if you start reading the input data of turn n+1 on the stdin without having sent a response in the stdout at turn n, the referee program will consider that your program did not respond in due time (timeout).

## Bot programming games
 
Bot programming games are multiplayer games with a game loop. Your goal is not to output a solution but to create a bot (an AI) capable of playing a game in the given environment. There are no test cases to pass.

You're required to submit your bot to the arena of the game to be ranked against other players. Our system automatically play matches between bots in the arena every time a new bot, or a new version of a bot is submitted.

Here's a [guide to get started in bot programming games](https://www.codingame.com/playgrounds/53785/tutorial-for-bot-programming-on-codingame). It's actually simpler than it looks!