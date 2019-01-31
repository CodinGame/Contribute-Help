A team of CodinGamers create a game/puzzle with the help of CodinGame. CodinGame then publishes it as an worldwide coding competition: a community contest, created by developers for developers.

CodinGame started organizing community contests in 2017. The first one, Mean Max, was published in November 2017. The full list of community contests can be found [here](pages/community/contest.md)

The creators of community contests are rewarded with a canvas of their game artwork, a CodinGame T-Shirt and are granted 2500 XP on the platform. Even if represents a certain amount of voluntary work, creating a contest as a CodinGamer is a fantastic achievement that anyone could be proud of.

# Creating a Contest

In average, it takes a few months to create a contest. Here are the different phases of creation:

- **Brainstorm**: CodinGamers regroup as they please and discuss ideas for a game or puzzle.
- **Prototype**: Once they agree on one or two ideas, they start prototyping using the [CodinGame Game Engine](https://github.com/CodinGame/codingame-game-engine), also known as CodinGame sdk. Once they're happy with one prototype, they submit it for CodinGame's review. The main point of contact is [CG]Thibaud (via the chat, Discord, or by email: thibaud@codingame.com)
- **Approval**: CodinGame reviews the prototype based on the guidelines below. If the prototype complies with the guidelines, the creators team must agree to work in collaboration with CodinGame to see their game/puzzle published as a contest. The creators team and CodinGame agree on a release date, name and theme for the contest. The contest is then announced to the community.
- **Development**: The creators team continues working on their game/puzzle, with CodinGame's support. The communication is done on a private channel in Discord. CodinGame takes care of the creation of the viewer assets and also the statement translation to French if needed.
- **Release**: CodinGame announces and releases the game. Bug fixing happens only at the beginning of a contest, except for game-breaking bugs.
- **Post-Contest**: The creators team can modify their game/puzzle for its future release as a non-competition.

# Rules

CodinGame contests engage CodinGame's brand. Therefore, CodinGame asks contributors to respect a few rules:

- The creators team must be ready to collaborate with CodinGame. _We're in this together_
- The creators team must be commited to the success of the project. _Once announced, the community expects the contest_
- CodinGame employees remain the final judges on all points. _We have the experience, trust us_
- No inappropriate content.

# Core Guidelines

CodinGame will review game/puzzle prototypes based on these core guidelines:

> Note: all recent contests have been AI games. These guidelines reflect this trend but everything is possible.

- Team
	- At least 2 contributors, no more than 4.
	- At least 1 contributor is confident with Java.
- Game
  - The game's core must be enough. No extra rules for the sake of complexity (e.g. no bonus pickups, no once-per-game boosts, no hero selection).
  - The game must be beginner-friendly (a bunch of ifs should make a workable AI).
  - The game must be fair
  	- Only the initial state of the game should be randomized (random things shouldn't be introduced during a game).
  	- Viable strategies must not include foul play (such as purposefully conflicting with opponent on evey turn) or idle play (such as just waiting).
  - The game should be fun and original.
- Prototype
  - The prototype should contain minimum features
  	- A basic viewer.
  	- A short statement (goal + protocol: In/Out).
  	- A valid [stub](/technical/stub.md).
  	- A default AI that does not immediately crash.
  	- A test AI (no hardcoding).

# General Guidelines

The following guidelines refer to a final game more than to a prototype. They should be respected as much as possible during the Development phase.

- Viewer
  - The viewer must be self-explanatory. _A player should understand most of the rules from a replay_
  - The viewer must contain the avatars and nicknames of current players (if multi).
- Referee
  - The referee must end a player's program when receiving an unrecognizable command.
  - The referee must send an error message in the console when receiving an invalid but recognized command.
  - The referee must stop the game early if the game is stale or already decided.
  - The referee must not crash. All exceptions must be caught (especially during the parsing of a Player’s actions, where most errors occur).
  - Indices must start at 0, not 1. The origin is always the top left pixel/tile.


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
- [Statement](technical/statement.md#game-statement)
  - The statement should not contain flavour text (clarity > style).
  - The statement should not address the reader directly (clarity > style).
  - The length of the statement should not exceed 6k characters.
- Graphics
  - The viewer should contain less than 20 shapes visible at once (rectangle, circle, etc.) or should use sprites.
  - Less than 2Mb in total should be used.
  - The minimum font size should be 36px.
  - The choice of colors should take into account color-blind people as much as possible.
- Viewer Prototype
  - :X: Don't
  <img src="https://admin.codingame.com/servlet/fileservlet?id=24927507397690" alt="bad prototype example" width="200"/>
  - :white_check_mark: Do
  <img src="https://admin.codingame.com/servlet/fileservlet?id=24927516490637" alt="good prototype example" width="200"/>