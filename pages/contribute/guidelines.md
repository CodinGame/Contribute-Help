# General Guidelines

- All types of games must have a clear and unambiguous description.

```- Keep it clear and consise

- Avoid flavour text

- Don't address the reader directly

- Avoid controversial topics
```

> - Keep it clear and consise
> - Avoid flavour text
> - Don't address the reader directly
> - Avoid controversial topics

 Check out the [statement guidelines](pages/technical/statement.md#guidelines) for more details.

- All types of games must have a working default code for all languages. Check out the [stub generator syntax](pages/technical/stub.md).

- Test cases must be properly defined.

> - Test cases should cover all specifications
> - Test cases must have explicit names
> - Each validator must differ from the correspond test
> - Each validator should check the same case as the corresponding test
> - The first test case must be a simple one

Check out the [test cases guidelines](pages/technical/testcase.md#guidelines) for more details.

|:---:|:---:|:---:|:---:|:---:|:---:|
|  | Clash of Code | In/Out Puzzle | Solo Puzzle | Optimization Puzzle | Multiplayer Game |
| Statement | X | X | X | X | X |
| Stub | X | X | X | X | X |
| Test Cases | X | X | X | X |  |
| Referee |  |  | X | X | X |
| Originality |  | X | X | X | X |


[Referee Guidelines](pages/types/game.md#guidelines)

# Specific Guidelines

## Clash of Code

- CoC puzzles should be solvable in less than 5 minutes.

_The main goal of a CoC battles is to be short (except in the "Shortest" mode). CoC players don't expect to learn something from solving a CoC puzzle; they'll choose practice puzzles for that._

- Close duplicates are allowed.

_If the puzzles' themes differ, it's ok to accept multiple versions of the same programming problem_

- No puzzle is too easy.

_No CoC puzzle should be rejected because it's too simple._


## Optimization Puzzles

- It must be very difficult to approach the optimal score.

## Multiplayer Games

- It's possible to write a working AI in a few minutes.

- If several leagues exist: boss difficulty is low but requires knowledge of each new set of rules per league.


