There are two different kinds of puzzles:

- **In/Out puzzles**: the most classic puzzle on CodinGame; compute a result once based on some input and send it in the output stream. Result is checked against test cases. They are built with a simple form.
- **Gameloop puzzles**: turn-based game, most of the times associated with a viewer; in an infinite loop, read the entries in the input stream and send an output to play the game. They are built with the CodinGame game engine (aka the sdk).

Learn how to write a statement [here](/technical/statement.md#puzzle-statement)

## Test Cases

Each test case has a test and a validator. Tests are visible to the participants whereas validators are hidden.

Each validator must be related (in terms of content) to its corresponding test but different at the same time to avoid hardcoding.

The first test must be simple because it will be included in the statement. Try to fill in the tests with an increasing level of difficulty.