**The following guidelines are what they are: guidelines. Please keep the experience of players in mind when creating/approving contributions.**

_Disagree with the current guidelines? Let us know in the [forum](https://www.codingame.com/forum/t/contribution-guidelines/112629)_

## General Guidelines

0. **Contributions must be written in English.**

1. **The description must be clear and unambiguous.** _(for all games but reverse CoC)_

	```
	- Keep it clear and consise
	- Avoid flavour text
	- Don't address the reader directly
	- Avoid controversial topics
	- Don't overlook the protocol
	```

 	=> [Writing the statement](pages/technical/statement.md#guidelines)

2. **The default code must be working for all languages.**

	=> [Stub generator syntax](pages/technical/stub.md)

3. **Test cases must be properly defined.** _(for all games with test cases)_

	```
	- Test cases should cover all specifications
	- Each validator must differ from the corresponding test
	- Each validator should check the same case as the corresponding test
	- The first test case must be a simple one
	```

	=> [Defining test cases](pages/technical/testcase.md#guidelines)

4. **Contributions must be original.** _(for all games but Clash of Code)_



## Specific Guidelines

### Clash of Code

The main goal of a CoC battle is to be solved in a short period of time. CoC players are looking for quick simple puzzles to solve; for more complex problems, they'll dive into the classic puzzles section.

1. **No CoC puzzle is too easy.**

	In theory, no CoC puzzle should be rejected with the justification that it's too simple. However, moderators should reach an agreement on whether a trivial CoC contribution is worth being added to the pool of CoCs.

2. **CoC close duplicates are not forbidden.**

	Moderators should reach an agreement on whether duplicate versions of a puzzle can be accepted or not. Copy-pasting an existing CoC puzzle is obviously not allowed.

3. **CoC statements should be self-sufficient.** (doesn't apply to reverse puzzles obviously)

	When your time is counted, as a player, you don't want to waste time searching for a formula or a definition online to understand what needs to be done.

4. **Binary or language-specific outputs should be avoided in CoC.**

	Some output formats favor specific languages and make the contribution unbalanced. Binary outputs open the door to "cheating" solutions to get around 50%.


### Optimization Puzzles

1. **It must be very difficult to approach the optimal score.**


### Games created with the sdk

1. **The referee program should be robust and reliable.**

	```
	- The referee must end a player's program when receiving an unrecognizable command.
	- The referee must send an error message in the console when receiving an invalid but recognized command.
	- The referee must stop the game early if the game is stale or already decided.
	- The referee must not crash. All exceptions must be caught.
	- Indices must start at 0, not 1. The origin is always the top left pixel/tile.
	```

2. **The graphics are clear and represent the progression of the game well.**

	```
	- The graphics must be self-explanatory. _A player should understand most of the rules from a replay_
  	- The graphics must contain the avatars and nicknames of current players (if bot programming).
  	```