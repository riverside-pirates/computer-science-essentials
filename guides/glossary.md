# Glossary

Plain words for the words in this course. Press `Ctrl+F` and type the word
you're hunting for. The current voyage's words come first, then Python words,
then everything else A–Z.

## Words for the Git Foundations voyage 🏴‍☠️

**autograder** — the robot that checks your Python every time your work
reaches `main` on GitHub. Scores show up in your repository's **Releases**
and in the **Feedback** pull request.

**branch (in Git)** — a separate line of work in your repository with its
own name, like `navigate-grid`. You commit on a branch, then open a pull
request to merge it into `main`. (For the other meaning, see
**branch (in a program)** below.)

**clone** — copy a repository from GitHub onto your computer so you can work
on it.

**codespace** — VS Code running in your browser on a GitHub computer, for
when you don't have your laptop. See [the Codespaces guide](codespaces.md).

**commit** — a saved snapshot of your changes, with a short note saying what
you did (like `Calculate rations`). Your commits are the record of your work.

**Feedback PR** — a pull request in your repository where Mr. B leaves
comments on your work. You read and reply there; you never merge it.

**GitHub** — the website where your repositories live and where work is
turned in. Your laptop has a copy of your repository; GitHub has the one
that counts.

**main** — the home branch of your repository. The autograder grades only
`main`, so your work is submitted when it lands there.

**merge** — bring the commits from one branch into another, usually by
merging a pull request into `main`.

**merge conflict** — two changes touched the same lines, so Git asks a human
to choose. VS Code shows both versions; pick, then commit. Nothing is lost.

**pull request (PR)** — a request to merge your branch into `main`, with a
page where a partner or teacher can comment and click **Approve**. In
git-03, each partner approves the other's PR.

**push** — send your commits from your laptop up to GitHub. In VS Code,
click **Sync Changes**. Until you push, GitHub and the autograder can't see
your work.

**repository (repo)** — one project's folder plus its entire history, on
GitHub and on your laptop.

**Source Control** — the VS Code panel (the branching icon on the left)
where you type a commit message, commit, and click **Sync Changes**.

**Sync Changes** — the VS Code button that pushes your commits to GitHub and
pulls down anything new. When in doubt, sync.

**terminal** — a text window where you type commands for the computer to
run, such as `git` or `python`. In VS Code, open one with
**Terminal → New Terminal**.

**tests** — the checks in your repository's `tests/` folder. Run them
yourself with `python -m pytest -q` before you push. `pytest` is the tool
that runs them.

**version control** — keeping the full history of changes to your files so
any version can be seen or brought back. Git is the version control tool
this class uses.

## Python words (from App Inventor to typed code)

See [Blocks to Python](blocks-to-python.md) for the full block-by-block map.

**argument** — a value you hand to a function when you call it. In
`food_needed(4, 3)`, the arguments are `4` and `3`.

**Boolean** — a value that is either `True` or `False` (capitalized in
Python).

**call** — run a function by writing its name with parentheses:
`food_needed(4, 3)`. The typed version of a `call` block.

**comparison operator** — `==`, `!=`, `<`, `>`, `<=`, `>=` (also called
relational operators). A comparison
gives back `True` or `False`. Careful: `==` compares, `=` assigns.

**def** — the keyword that starts a function:
`def food_needed(crew, days):`. The typed version of a `to ...` block.

**elif** — "else if": the next check in a chain of `if` tests. Python tries
each test in order until one is `True`.

**f-string** — a string that fills in values: `f"Crew of {crew}"` puts the
value of `crew` into the text.

**function** — a named chunk of code that does one job and can be called
again and again. Like a procedure block in App Inventor.

**indentation** — the 4 spaces that push a line to the right. Indenting is
Python's version of tucking blocks inside a block. Lines at the same indent
level form a block.

**parameter** — a name inside the parentheses of a `def` that receives an
argument. In `def food_needed(crew, days):`, the parameters are `crew` and
`days`.

**return** — hands a result back to whoever called the function. The typed
version of the `result` socket.

**string** — text in quotes: `"Hello "`. A piece of one is a substring.

**variable** — a name that stores a value: `speed = 3`. Like
`initialize global speed to 3`, in one line. The `get speed` block is just
`speed`, and `set speed to` becomes `speed = ...`.

## Everything else, A–Z

**abstraction** — hiding the details so you can think about the big idea. A
function you can call without reading its insides is an abstraction.

**accessibility** — how usable a program is for people with different
abilities.

**accumulator** — a variable that keeps a running total: set it up before a
loop, add to it inside the loop, use the total after.

**algorithm** — a set of steps that accomplishes a task. You can write one
as code, pseudocode, a flowchart, or plain language.

**app** — a software application, especially one you download to a phone or
tablet.

**append** — add an element to the end of a list. In Python:
`crew.append("Polly")`.

**application programming interface (API)** — the published rules for how to
use someone else's code or service: what to call, what you get back.

**arithmetic operator** — a symbol that does math: `+`, `-`, `*`, `/`.

**array** — an ordered collection of elements, all the same type. Python's
version is the list.

**artificial intelligence (AI)** — machines showing behavior that seems
intelligent.

**assignment** — storing a value in a variable with `=`, as in
`color = 255`. (The other kind of assignment is on
[classroom50.org](https://classroom50.org).)

**authenticate** — prove who you are to a computer, like signing in with
`gh student login`.

**authorized hacking** — testing a system's defenses with permission, to
find and fix weaknesses.

**backlog** — the prioritized to-do list for building an app.

**bash** — a shell: a program that takes typed commands and runs them. One
of several languages a terminal can speak.

**best-so-far loop** — a loop that keeps a variable holding the best value
seen yet, replacing it whenever a better one shows up.

**block (in Python)** — the lines at the same indentation level, which run
together.

**block (in App Inventor)** — a puzzle piece you snap into a program instead
of typing. Blocks control the components you placed in the Design view,
like Button and Label. A language made of these is a block-based (visual)
programming language.

**Boolean expression** — a test that comes out `True` or `False`, like
`x > 0`.

**brainstorming** — a group throwing out ideas freely before judging any of
them.

**branch (in a program)** — an alternate path the program can take,
usually chosen by an `if`. (For Git branches, see the voyage words above.)

**broadcast** — a signal one part of a program sends to start an event or
procedure in another part.

**brute force attack** — guessing passwords over and over until one works.

**CamelCase** — naming style that marks new words with capitals instead of
spaces: `StudentProject` or `studentProject`.

**Cascading Style Sheets (CSS)** — the language that describes how a web
page should look in the browser.

**character** — a single letter, digit, or symbol you can type: `a`, `7`,
`?`.

**class** — a template for making objects: it defines their data
(attributes) and their behaviors (methods). An object made from a class is
an instance of it.

**cloud computing** — using computers you reach over the internet, instead
of your own, to store and process data.

**code** — the instructions in a program.

**collaboration** — two or more people working toward one goal by sharing
the work and the ideas.

**compiler** — a program that translates human-readable code into the 0s
and 1s a computer actually runs.

**complex conditional** — one `if` test built from several conditions,
joined with `and`, `or`, or `not`.

**computer science** — solving problems and building things with the power
of a computer: programming, algorithms, data, graphics, and more.

**computer system** — computers and programs working together for one
purpose.

**concatenation** — joining pieces into one, without changing them.
`"Hello " + "world!"` (note the space in `"Hello "`) gives
`"Hello world!"`.

**conditional statement** — code that does different things depending on
whether a test is `True` or `False`: `if`, `elif`, `else`. A chain of these
is a chained conditional. The test itself is a conditional expression.

**consensus** — general agreement in a group.

**counting loop** — a loop that counts up or down with each pass, often to
control how many times it runs.

**data type** — what kind of data a value is: string, integer, float,
Boolean. The type limits what values are allowed. In a variable, it's the
kind of data stored there.

**debug** — find the errors (bugs) in a program and fix them.

**decomposition** — breaking a big problem into smaller parts that are
easier to understand and build. Also called problem decomposition.

**decrement** — decrease a value, usually by 1. The opposite of increment.

**design** — plan how a program will meet its goal before building it.

**development process** — building in rounds: make a version, test it, get
feedback, improve it, repeat.

**diameter** — the distance straight across a circle through its center.

**domain name** — the owned part of a web address, like `github.com`. Its
ending (`.com`, `.org`, `.edu`, `.gov`) is the top-level domain.

**dynamic** — describes a program whose behavior changes with its inputs
and conditions.

**equality** — testing whether two values are the same, with `==`. `8 == 8`
is `True`.

**event** — something that happens (a click, a key press, a timer) that a
program can react to. The code that reacts is an event handler. A program
built this way — nothing runs until something happens — is event-based.

**exploit** — software or commands that take advantage of a weakness in a
system to make it misbehave.

**expression** — a combination of values, variables, and operators that
works out to a single value, like `crew * days * 2`.

**feature** — one thing an app can do.

**file extension** — the end of a filename after the last dot (`.py`,
`.md`), which tells you the file type.

**file path** — the directions to a file, like
`guides/glossary.md`.

**float** — a number with a decimal point, like `3.14`. Limited precision:
it can only hold so many decimal places accurately.

**flowchart** — a diagram of a program's paths using shapes and arrows.

**for loop** — a loop that runs a known number of times, like once per item
in a list. (Compare the while loop, which runs as long as a condition holds.)

**generative AI** — AI that learns patterns from existing data and uses
them to produce new text, images, music, or code.

**global variable** — a variable usable anywhere in the program. (Compare
local variable.)

**hack** — use technology to get access you wouldn't otherwise have.

**hacker** — either a criminal who breaks into systems, or a clever
programmer who finds weaknesses to fix them. Context decides which.

**hard coding** — writing fixed values straight into the code, so the
program can't change without editing the code itself.

**high-level programming language** — a language like Python that hides
machine details so humans can write code faster. (A low-level language is
near the 0s and 1s the machine runs.)

**import statement** — a line that pulls someone else's code (a module or
library) into your program: `import math`.

**increment** — increase a value, usually by 1. A loop that counts events
this way is an incremental counter.

**index** — an item's position number in a list. Python counts from 0; App
Inventor counts from 1.

**initialize** — give a variable its first value. Before that, it doesn't
exist yet.

**innovation** — improving something that exists into something more
useful.

**input** — data given to a program while it runs: clicks, keys, touches,
sensor readings (light, distance, touch, like App Inventor's Sensors
drawer), arguments.

**integer** — a whole number, no decimal: `42`.

**integrated development environment (IDE)** — one app for writing,
running, and debugging code. VS Code is this class's IDE.

**interpreted language** — a language like Python whose instructions can
run one at a time, without compiling the whole program first.

**iteration** — one pass through a loop; also the looping itself.

**list** — an ordered collection of items. Each item (a list element) sits
at a position called its index and can be any data type.

**local variable** — a variable that exists only inside one part of the
program, like inside one function. (Compare global variable.)

**logic** — the decision-making in a program: testing conditions to choose
what happens next.

**logical operator** — `and`, `or`, `not`: combines or flips `True`/`False`
values.

**loop** — a structure that repeats instructions. Each repeat is an
iteration, usually controlled by a condition.

**method** — a function that belongs to an object, called with a dot:
`crew.append("Polly")`.

**mobile application** — an app that runs on a device you carry.

**modular** — built from pieces that each do their own job and connect
simply, so one piece can change without rewriting the rest.

**modulo** — the `%` operator: divides and gives back the remainder.
`7 % 2` is `1`.

**natural language** — the language people speak with each other, as
opposed to a programming language.

**nesting** — putting one structure inside another: a loop in a loop, an
`if` in an `if`.

**object** — one specific thing made from a class, with its own attribute
values, able to run its class's methods.

**object-oriented programming** — a style of programming built around
classes and objects, so code patterns can be reused.

**one-dimensional array** — a single line of elements, all the same type.
(A two-dimensional one adds rows and columns.)

**online code editor** — a programming environment in the browser, nothing
to install. Your codespace is one.

**open-ended problem** — a problem with many possible good answers, not one
correct one. (One that's also hard to even pin down is ill-defined.)

**operand** — a value an operator works on. In `5 + 2`, the operands are
`5` and `2`.

**operating system (OS)** — the software that runs the computer itself.
Your laptops run Windows 11; Ubuntu is a free OS your codespace runs.

**output** — what a program produces: text, graphics, sound, actions.

**pair programming** — two people, one keyboard: the driver types, the
navigator directs, and you switch often.

**pi** — the ratio of a circle's circumference to its diameter, about 3.14.

**prepend** — add to the beginning. (Compare append.)

**primary source** — the original work itself. A secondary source
summarizes or comments on primary sources and cites them.

**problem solving** — working through a hard problem step by step instead
of guessing.

**procedure** — a named group of instructions a program can run on demand —
what Python calls a function. Using one while only knowing *what* it does,
not *how*, is procedural abstraction.

**processor** — the computer chip that does the computing: it takes input
data in and sends results out. It's built from billions of tiny on/off
switches called transistors.

**professional** — behaving, dressing, and communicating in a way that
respects everyone in the room.

**program documentation** — written explanation of what code does and how
it was built, for the next person who reads it.

**protocol** — an agreed-upon way for computers to talk to each other.

**pseudocode** — the steps of an algorithm written in plain language before
real code.

**Python** — the text-based programming language this class uses, designed
to be readable and brief.

**Python interactive interpreter** — also called the Python shell: the mode
where you type Python one
line at a time and see each result immediately. Start it by typing `python`
in the terminal; the `>>>` prompt means it's waiting for you. It isn't
bash: bash runs computer commands, the interpreter runs Python.

**radius** — the distance from a circle's center to its edge.

**range** — Python's counting function for loops:
`range(start, stop, step)`. `for day in range(3):` runs 3 times.

**rendering** — turning code and data into what you see on the screen.

**RGB color model** — mixing red, green, and blue light, each 0–255, to
make any screen color. 0 is none of that color; 255 is all of it.

**scope** — the parts of a program where a variable can be seen and
changed.

**Scrum** — a team development process that builds in short rounds
(sprints) with feedback from stakeholders. The Scrum Master keeps the
process running and removes obstacles; the product owner keeps the
requirements; each sprint has its own small-task list.

**Scrum poker** — a team estimating game: everyone picks an effort estimate
privately, then all reveal at once, so nobody anchors on the first number
said aloud.

**server** — a computer that many users share over a network, holding
files, apps, or databases. GitHub runs on servers.

**skeleton code** — a program with pieces deliberately missing for you to
fill in, usually with comments marking where.

**statement** — the smallest runnable piece of code, usually one line.

**substring** — a piece of a string.

**syntax** — a language's rules for what counts as correctly written code:
grammar for programs.

**team** — people with different strengths working toward one goal. Team
norms are the working agreements they set for themselves.

**Turing Award** — the "Nobel Prize of Computing," given yearly for major
contributions to computer science. Named for Alan Turing (1912–1954).

**two-dimensional array (2D array)** — an array with rows and columns; you
need both to find an element.

**type** — see **data type**.

**underscore case (snake_case)** — naming style that replaces spaces with
underscores, all lowercase: `food_needed`. Python's usual style.

**uniform resource locator (URL)** — a web address: the exact directions to
one resource on the internet.

**usability** — how easily a user can use an app without outside help.

**user** — the person the program is for. User-centric design keeps
checking with them: a user story describes one thing they need, and
developers build those in priority order.

**user interface** — the part of a program a user sees and interacts with.

**value** — a piece of data a program can store or work with.

**virtual machine** — a computer simulated in software. Your codespace runs
on one.

**while loop** — a repeating `if`: it keeps running its block as long as
its condition stays `True`.
