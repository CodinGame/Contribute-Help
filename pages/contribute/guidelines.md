# General Guidelines

0. **Contributions must be written in English.**

1. **The description must be clear and unambiguous.**

	```
	- Keep it clear and consise
	- Avoid flavour text
	- Don't address the reader directly
	- Avoid controversial topics
	```

 	=> [Statement guidelines](pages/technical/statement.md#guidelines)

2. **The default code must be working for all languages.**

	=> [Stub generator syntax](pages/technical/stub.md).

3. **Test cases must be properly defined.** _(for all games but multiplayer games)_

	```
	- Test cases should cover all specifications
	- Test cases must have explicit names
	- Each validator must differ from the correspond test
	- Each validator should check the same case as the corresponding test
	- The first test case must be a simple one
	```

	=> [Test cases guidelines](pages/technical/testcase.md#guidelines)

4. **Contributions must be original.** _(for all games but Clash of Code)_

5. **The referee program should be robust and reliable.** _(for all games created with the sdk)_

	```
	- The referee must end a player's program when receiving an unrecognizable command.
	- The referee must send an error message in the console when receiving an invalid but recognized command.
	- The referee must stop the game early if the game is stale or already decided.
	- The referee must not crash. All exceptions must be caught.
	- Indices must start at 0, not 1. The origin is always the top left pixel/tile.
	```

	=> [Referee Guidelines](pages/types/game.md#guidelines)

6. **The graphics are clear and represent the progression of the game well.** _(for all games created with the sdk)_


# Specific Guidelines

## Clash of Code

7. CoC puzzles should be solvable in less than 5 minutes.

_The main goal of a CoC battles is to be short (except in the "Shortest" mode). CoC players don't expect to learn something from solving a CoC puzzle; they'll choose practice puzzles for that._

8. Close duplicates are allowed.

_If the puzzles' themes differ, it's ok to accept multiple versions of the same programming problem_

9. No puzzle is too easy.

_No CoC puzzle should be rejected because it's too simple._


## Optimization Puzzles

10. It must be very difficult to approach the optimal score.


