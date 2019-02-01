The statement should be written **in English**. Make it as **clear and consise** as possible.

# Puzzle Statement
_(In/Out puzzle and CoC only)_

The statement of a puzzle describes the problem that the players have to solve.

## Syntax

<<Bold>> [[Variable]] {{Constant}} renders as:

`Monospace` renders as:

## The Story (non-mandatory)

Keep it short. It should serve the puzzle, not the contrary.

Avoid controversial topics like politics.

## The Goal

A short description of the goal of the puzzle: 1 or 2 sentences maximum.

Ex: _You must output the closest pair of points (euclidean distance)._

## The Rules

Explain how the puzzle works and what players are supposed to read from the input and send in output. Keep it concise: give the minimum amount of information needed to solve the problem.

## Input Description
Describe line by line, what must be read from standard input.

Ex: _<<Line 1:>> An integer [[N]] for the number of points to compare.
<<Next [[N]] lines:>> Two space separated integers [[x]] and [[y]] for the coordinates of a point._

## Output Description
Describe line by line, what must be written to the standard output.

Ex: _<<Line 1 :>> The coordinates of the point from the closest pair of points in the same order as given in input.
<<Line 2 :>> The coordinates of the other point from the closest pair of points._

## Constraints
Describe the variable constraints if you think they are needed to solve the problem.

Ex: _2 ≤ [[N]] ≤ 100
-1000 < [[x]],[[y]] < 1000_

# Game Statement
_(For all sdk games)_

For all games created with the sdk, the statement is an html document. You can find a default one [here](https://github.com/CodinGame/game-skeleton/blob/master/config/statement_en.html)

It should contain:

1. A quick description of the goal: 1 or 2 sentences maximum.
2. A list of rules to explain how the puzzle/game works
3. The Victory/Lose conditions
4. The protocol
	- the Input description
	- the Output description
	- a list of constraints
5. An example of Intput/Output
6. (non-mandatory) A story

## Guidelines <a name="guidelines"/>

- Keep it simple and consise
_A long statement can scare players away._
- Avoid flavour text
_For instance, **don’t say** “The unit hits the other unit on the nose, causing 1 point of excruciating damage”, do say “The unit deals 1 damage”._
- Don't address the reader directly
_For instance **don’t say** “This next part looks complicated but you’ll get it, don’t worry!”._
- Length < 6k characters

## Leagues

There are one statement file per leagues. They're all generated from one general statement file (/config/statement_en.html.tpl) when building the project.

## Conditional logic

To show a piece of statement only in the league _x_, write

```html
<!-- BEGIN levelx -->
	Piece of statement.
<!-- END -->```

To highlight a new rule, use the same as above with the following div style:

```html
<!-- BEGIN levelx -->
<div style="color: #7cc576;
        background-color: rgba(124, 197, 118,.1);
        padding: 2px;">
    Piece of statement.
</div>
<!-- END -->```




