A team of CodinGamers create a game/puzzle with the help of CodinGame. CodinGame then publishes it as an worldwide coding competition: a community contest, created by developers for developers.

CodinGame started organizing community contests in 2017. The first one, Mean Max, was published in November 2017. The full list of community contests can be found [here](pages/community/contest.md)

The creators of community contests are rewarded with a canvas of their game artwork, a CodinGame T-Shirt and are granted 2500 XP on the platform. Even if represents a certain amount of voluntary work, creating a contest as a CodinGamer is **a fantastic achievement that anyone could be proud of**.

# Creating a Contest

In average, it takes a few months to create a contest. Here are the different phases of creation:

1. **Brainstorm**: CodinGamers regroup as they please and discuss ideas for a game or puzzle.
2. **Prototype**: Once they agree on one or two ideas, they start prototyping using the [CodinGame Game Engine](https://www.codingame.com/playgrounds/25775/codingame-sdk-documentation), also known as CodinGame sdk. Once they're happy with one prototype, they submit it for CodinGame's review. The main point of contact is [CG]Thibaud (via the chat, Discord, or by email: thibaud@codingame.com)
3. **Approval**: CodinGame reviews the prototype based on the guidelines below. If the prototype complies with the guidelines, the creators team must agree to work in collaboration with CodinGame to see their game/puzzle published as a contest. The creators team and CodinGame agree on a release date, name and theme for the contest. The contest is then announced to the community.
4. **Development**: The creators team continues working on their game/puzzle, with CodinGame's support. The communication is done on a private channel in Discord. CodinGame takes care of the creation of the viewer assets and also the statement translation to French if needed.
5. **Release**: CodinGame announces and releases the game. Bug fixing happens only at the beginning of a contest, except for game-breaking bugs.
6. **Post-Contest**: The creators team can modify their game/puzzle for its future release as a non-competition.

# Rules

CodinGame contests engage CodinGame's brand. Therefore, CodinGame asks contributors to respect a few rules:

- The creators team must be ready to collaborate with CodinGame. _We're in this together_
- The creators team must be commited to the success of the project. _Once announced, the community expects the contest_
- CodinGame employees remain the final judges on all points. _We have the experience, trust us_
- No inappropriate content.

# Guidelines

CodinGame will review game/puzzle prototypes based on these following core guidelines:

> Note: all recent contests have been AI games. These guidelines reflect this trend but everything is possible.

- **Team**
	- At least 2 contributors, no more than 4.
	- At least 1 contributor is confident with Java.
- **Game**
  - The game's core must be enough. No extra rules for the sake of complexity (e.g. no bonus pickups, no once-per-game boosts, no hero selection).
  - The game must be beginner-friendly (a bunch of ifs should make a workable AI).
  - The game must be fair
  	- Only the initial state of the game should be randomized (random things shouldn't be introduced during a game).
  	- Viable strategies must not include foul play (such as purposefully conflicting with opponent on evey turn) or idle play (such as just waiting).
  - The game should be fun and original.
- **Prototype**
  - The prototype should contain minimum features
  	- A basic viewer.
  	- A short statement (goal + protocol: In/Out).
  	- A valid [stub](/technical/stub.md).
  	- A default AI that does not immediately crash.
  	- A test AI (no hardcoding).

During the Developement phase, [general guidelines](pages/types/ai.md#guidelines) and [best practices](pages/types/ai.md#best-practices) should be respected.

## Viewer Prototype

<img src="https://admin.codingame.com/servlet/fileservlet?id=24927507397690" alt="bad prototype example" style="width:200px;"/>❌ Don't</img>
<img src="https://admin.codingame.com/servlet/fileservlet?id=24927516490637" alt="good prototype example" width="200"/>✅ Do</img>