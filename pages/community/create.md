All content on CodinGame is published under the following license:
[License CC BY-SA 2.0](https://creativecommons.org/licenses/by-sa/2.0/)

## Contribution Process

A contribution has 3 different states:

- **Private**: a draft that can be shared with friends with the link.
- **WIP**: as Work In Progress. Visible by everyone for feedback and suggestions but not yet ready to be approved and published. WIP contributions cannot be approved. Unless the author changes its state, a WIP contribution goes back to a private state after 30 days.
- **Ready**: visible by everyone and ready for approval. If a ready contribution is not approved/rejected after 30 days, it goes back to a private state. A contribution cannot be published before 7 days even if it has been approved 3 times, to let time for other moderators to review it. If during this period it is rejected 3 times, it will go back to a private state, even if 3 moderators approved it.

To submit a classic puzzle or CoC puzzle as *WIP* or *Ready*, the author must provide a solution to the puzzle, in any language.

It's highly recommended:
- to solve enough puzzles before trying to create your own
- to publish a contribution as "WIP" first to get feedback from the community. 

=> [More details about the approval process](pages/community/approval.md)

### XP Rewards

Contributing to CodinGame rewards with XP.

- Every time one of your contribution us upvoted, you'll get 10 XP.
- Every time one of your contributions is (definitely) approved, you'll get 250 XP.
- Every time one of your comments is upvoted, you'll get 1 XP.

## Types of contributions

Here is what you can create on CodinGame:

1. [In/Out Puzzles](/pages/basics/puzzle.md)
_(created via a form on CodinGame)_
	- Classic Puzzle
	- Clash of Code puzzle
2. [Coding Games](/pages/basics/game.md)
_(created with the CodinGame Game Engine, also known as the sdk)_
	- Solo Game
	- Multiplayer Game (Bot Programming)
	- Optimization Game

<img src="https://www.codingame.com/servlet/mfileservlet?id=66584542418448" width="400" style="margin-left: auto;margin-right: auto;display: block;">

## Other types of contributions

Contributing to CodinGame isn't only about creating new puzzles/games. It's also about:

- helping others in the [community spaces](pages/community/chat.md)
- sharing your knowledge
- reviewing other's contributions and commenting
- writing [articles/playgrounds](pages/community/article.md)

You can find [here, a list of useful tools](pages/community/tool.md) created by community members.

Some community members also participated in the creation of community challenges from 2017 to 2020. Find [the complete list of challenges here](pages/community/contest.md). At that time, you could also enjoy [joining a CodingHub](pages/community/hub.md)

## Best Practices

### Coding Games

When creating a coding game, we suggest you follow these best practices in order to improve both its performance and the players' experience.

- **Protocol/Stub**
  - If options for a player are limited, they should be sent in input (ex: [Wondev Woman](https://www.codingame.com/ide/puzzle/wondev-woman))
  - The player's id should be 0.
  - The player's input should be sent first in loops.
  - Any non-explicit variable should be explained with a comment.
  - The stub should not change between leagues.
  - The generated stub should not contain more than 45 lines in Java.
  - The number of variables per loop should not exceed 10.
  - There should be a maximum of 2 loops.
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
