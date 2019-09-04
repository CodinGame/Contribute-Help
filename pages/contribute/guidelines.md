It's highly recommended to publish a contribution as "WIP" first to get feedback from the community. 
=> [More details about moderation](pages/contribute/moderation.md)

**The following guidelines are what they are: guidelines. Please keep the experience of players in mind when creating/moderating contributions.**

_Disagree with the current guidelines? Let us know in the [forum](https://www.codingame.com/forum/t/contribution-guidelines/112629)_

# General Guidelines

0. **Contributions must be written in English.**

1. **The description must be clear and unambiguous.** _(for all games but reverse CoC)_

	```
	- Keep it clear and consise
	- Avoid flavour text
	- Don't address the reader directly
	- Avoid controversial topics
	_ Don't overlook the protocol
	```

 	=> [Writing the statement](pages/technical/statement.md#guidelines)

2. **The default code must be working for all languages.**

	=> [Stub generator syntax](pages/technical/stub.md)

3. **Test cases must be properly defined.** _(for all games but multiplayer games)_

	```
	- Test cases should cover all specifications
	- Test cases must have explicit names (for all tests but CoC validators)
	- Each validator must differ from the corresponding test
	- Each validator should check the same case as the corresponding test
	- The first test case must be a simple one
	```

	=> [Defining test cases](pages/technical/testcase.md#guidelines)

4. **Contributions must be original.** _(for all games but Clash of Code)_

5. **The referee program should be robust and reliable.** _(for all games created with the sdk)_

	```
	- The referee must end a player's program when receiving an unrecognizable command.
	- The referee must send an error message in the console when receiving an invalid but recognized command.
	- The referee must stop the game early if the game is stale or already decided.
	- The referee must not crash. All exceptions must be caught.
	- Indices must start at 0, not 1. The origin is always the top left pixel/tile.
	```

	=> [Games guidelines and best practices](pages/types/game.md#guidelines)

6. **The graphics are clear and represent the progression of the game well.** _(for all games created with the sdk)_


# Specific Guidelines

## Clash of Code

1. **CoC puzzles should be solvable in less than 5 minutes.**

	The main goal of a CoC battles is to be short (except in the "Shortest" mode). CoC players are looking for quick simple puzzles to solve; for more complex problems, they'll dive into the classic puzzles section.

2. **CoC close duplicates are allowed.**

	If the puzzles' themes differ, it's ok to accept multiple versions of the same programming problem. _(to a maximum of 5 duplicates)_

3. **No CoC puzzle is too easy.**

	No CoC puzzle should be rejected because it's too simple. _(to the limit of overly-simple puzzles which can feel unrewarding/unenjoyable)_


## Optimization Puzzles

1. **It must be very difficult to approach the optimal score.**


