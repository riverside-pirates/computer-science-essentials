# Blocks to Python

Same ideas you used in App Inventor, typed instead of snapped together. Each
day adds a few more blocks. Scroll up any time to review earlier days.

## Two rules for every day

**Two kinds of blocks.** Blocks that plug in from the **side** (math, compare,
`get`, `join`, and a `call` that gives a result) become values *inside* a line
of Python. Blocks that **stack** top to bottom (`set`, `if`) become whole lines.

**Indenting replaces nesting.** A block tucked inside another becomes a line
pushed right by 4 spaces, the way blocks sit inside a procedure or an `if`.

## Day 1

| App Inventor block | Python |
| --- | --- |
| `initialize global  speed  to  3` | `speed = 3` |
| `get global speed` | `speed` |
| math `+`  `-`  `×` | `+`  `-`  `*` |
| `to  water_needed  crew  days  result` | `def water_needed(crew, days):` |
| the `result` socket | `return ...` |
| `call  water_needed  4  3` | `water_needed(4, 3)` |
| compare `=`  `≠` | `==`  `!=` |
| compare `<`  `>`  `≤`  `≥` | `<`  `>`  `<=`  `>=` |
| `true`  `false` | `True`  `False` |

**Watch it run.** [Open the example in Python Tutor](https://pythontutor.com/visualize.html#code=WATER_PER_PERSON_PER_DAY%20%3D%202%0A%0Adef%20water_needed%28crew%2C%20days%29%3A%0A%20%20%20%20return%20crew%20%2A%20days%20%2A%20WATER_PER_PERSON_PER_DAY%0A%0Atotal%20%3D%20water_needed%282%2C%203%29%0Aprint%28total%29%0A&mode=edit&py=311), click
**Visualize Execution**, then click **Next >** to go one line at a time.

## Day 2

| App Inventor block | Python |
| --- | --- |
| `initialize local  new_x  to  get x` | `new_x = x` (inside a function) |
| `set  new_y  to  + (get y, get steps)` | `new_y = y + steps` |
| `if` with an **else if** socket (blue gear) | `if ...:` then `elif ...:` |
| compare texts `=` | `==`, for example `direction == "N"` |
| `make a list  new_x  new_y` | `(new_x, new_y)`, which is a **tuple** |
| `and`  `or`  `not` | `and`  `or`  `not` |
| two compares joined by `and` | `1 <= n <= 20` |
| `is number?` | `type(n) == int` (whole numbers only) |

**`elif` lines up under `if`**, and the line it controls is indented 4 spaces
under the `elif`:

```python
if direction == "N":
    new_y = y + steps
elif direction == "S":
    ...
```

**Text isn't a number in Python.** App Inventor's `is number?` says yes to
`"3"`. Python doesn't: `type("3") == int` is `False`. That's why `on_chart`
checks the type first.

**Watch it run.** [Open the example in Python Tutor](https://pythontutor.com/visualize.html#code=def%20move%28x%2C%20y%2C%20direction%2C%20steps%29%3A%0A%20%20%20%20new_x%20%3D%20x%0A%20%20%20%20new_y%20%3D%20y%0A%20%20%20%20if%20direction%20%3D%3D%20%22N%22%3A%0A%20%20%20%20%20%20%20%20new_y%20%3D%20y%20%2B%20steps%0A%20%20%20%20return%20%28new_x%2C%20new_y%29%0A%0Aposition%20%3D%20move%282%2C%203%2C%20%22N%22%2C%204%29%0Aprint%28position%29%0A&mode=edit&py=311), click
**Visualize Execution**, then click **Next >** to go one line at a time.

## Day 3

| App Inventor block | Python |
| --- | --- |
| `join  "Cargo: "  get item` | `f"Cargo: {item}"` (an **f-string**) |
| `if` / `else` filling the `result` socket | `if ...:` / `else:`, with a `return` in each |
| `call  format_location  x  y` inside another procedure | `format_location(x, y)` inside another function |
| a block from another drawer | `from navigator import format_location` |

**f-strings:** put `f` before the quote, and put values inside `{ }`.
Everything else is copied exactly, spaces included.

```python
count = 3
f"Cargo: rope x{count}"      # gives "Cargo: rope x3"
```

**You can call functions inside the braces:**

```python
f"{format_cargo('rope', 3)} | {hull_status(0)}"
# gives "Cargo: rope x3 | Hull OK"
```

**Watch it run.** [Open the example in Python Tutor](https://pythontutor.com/visualize.html#code=def%20format_cargo%28item%2C%20count%29%3A%0A%20%20%20%20return%20f%22Cargo%3A%20%7Bitem%7D%20x%7Bcount%7D%22%0A%0Adef%20hull_status%28damage%29%3A%0A%20%20%20%20if%20damage%20%3D%3D%200%3A%0A%20%20%20%20%20%20%20%20return%20%22Hull%20OK%22%0A%20%20%20%20else%3A%0A%20%20%20%20%20%20%20%20return%20f%22Hull%20damaged%20by%20%7Bdamage%7D%22%0A%0Areport%20%3D%20f%22%7Bformat_cargo%28%27rope%27%2C%203%29%7D%20%7C%20%7Bhull_status%284%29%7D%22%0Aprint%28report%29%0A&mode=edit&py=311), click
**Visualize Execution**, then click **Next >** to go one line at a time.

## Want more?

The official Python tutorial:
[numbers and text](https://docs.python.org/3/tutorial/introduction.html) ·
[`if` statements and functions](https://docs.python.org/3/tutorial/controlflow.html) ·
[f-strings](https://docs.python.org/3/tutorial/inputoutput.html)
