The statement should be written **in English** and be as **clear and concise** as possible.

A typical statement contains:

1. A quick description of the goal: 1 or 2 sentences maximum.
2. A list of rules to explain how the puzzle/game works.
3. The Winning/Losing conditions (for games created with the SDK only).
4. The protocol
	- input parameters and their types
	- expected output
	- reasonable constraints

A theme/story is non-mandatory.

## <a name="guidelines"></a> Guidelines to write good statements

The statement must be clear and non-ambiguous.

- Keep it clear and concise

_A long statement can scare players away._

- Avoid flavour text

_For instance, **don’t say** “The unit hits the other unit on the nose, causing 1 point of excruciating damage”, do say “The unit deals 1 damage”._

- Don't address the reader directly

_For instance **don’t say** “This next part looks complicated but you’ll get it, don’t worry!”._

- Avoid controversial topics like politics.

- Don't overlook the protocol

_It must be clear, precise, with reasonable constraints..._

## <a name="puzzle-statement"></a> Puzzle Statement
_(In/Out puzzle and CoC only)_

### Syntax

\<\<Bold\>\> [[Variable]] {{Constant}} renders as:

<img src="https://static.codingame.com/servlet/fileservlet?id=2208548269998" alt="statement syntax img" width="200"/>

\`Monospace\` renders as: `Monospace`

### Example

```Goal:

You must output the closest pair of points (euclidean distance).


Input:

<<Line 1:>> An integer [[N]] for the number of points to compare.

<<Next [[N]] lines:>> Two space separated integers [[x]] and [[y]] for the coordinates of a point.


Output:

<<Line 1 :>> The coordinates of the point from the closest pair of points in the same order as given in input.

<<Line 2 :>> The coordinates of the other point from the closest pair of points.


Constraints:

2 ≤ [[N]] ≤ 100

-1000 < [[x]],[[y]] < 1000
```

The statement is limited to 5k characters.

## Game Statement
_(For all sdk games)_

For all games created with the sdk, the statement is an html document. You can find a default one [here](https://github.com/CodinGame/game-skeleton/blob/master/config/statement_en.html)

### Leagues

There is one statement file per league. They're all generated from one general statement file (located here: /config/statement_en.html.tpl) when building the project.

### Conditional logic

To show a piece of statement only in league _x_, write

```html
<!-- BEGIN levelx -->
	Piece of statement.
<!-- END -->
```

To highlight a new rule, use the same as above with the following div style:

```html
<!-- BEGIN levelx -->
<div style="color: #7cc576;
        background-color: rgba(124, 197, 118,.1);
        padding: 2px;">
    Piece of statement.
</div>
<!-- END -->
```




