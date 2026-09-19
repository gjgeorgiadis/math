# Math Lab

A set of browser math games for a young child who likes playing with numbers. Every file is a
self-contained HTML page — no build step, no libraries, no network calls. Open `index.html` to play.

```
index.html             the games page: unlocked games, math pictures, grown-ups panel
brick-pyramids.html    1  adding, subtracting, reasoning backwards, early algebra
pattern-machine.html   2  sequences and rules
googol-zoom.html       3  powers of ten, googol, googolplex
brick-fit.html         4  spatial reasoning
take-away.html         5  strategy (Nim)
gear-lab.html          6  gear ratios
mystery-machine.html   7  functions: probe, conjecture, predict
target-builder.html    8  open-ended search with + − × ÷
how-many-ways.html     9  combinatorics
balance-scale.html    10  equations and two unknowns
prime-factory.html    11  factors, primes, the sieve
binary-lights.html    12  base 2
below-zero.html       13  negative numbers
fraction-bricks.html  14  fractions
```

Each game unlocks when **Level 5** of the one before it is cleared, in the order above.

Progress is saved in the browser under the key `mathLab.v1`, so the pages must be served from one
place (a GitHub Pages site, a local web server) for unlocks to carry from the index to the games.

---

## How a game works

**Levels.** Each game has 10 levels plus an Endless mode. A level is a round of 8 puzzles.

**Clearing a level.** A puzzle counts as *perfect* only if it is solved with no wrong tries and no
hint. 5 perfect out of 8 clears the level (⭐), 6 earns ⭐⭐, 7–8 earns ⭐⭐⭐. Fewer than 5 means
"keep practicing" and the level can be replayed.

**Express Pass.** If the first 5 puzzles of a round are all perfect, the round ends there with 3
stars. This is the escape hatch for levels the child has already mastered — he can climb to his real
level in a few minutes instead of grinding through easy questions.

**Help while playing.** A wrong answer shakes and says so. After 2 wrong tries a hint appears (tap 💡
for it sooner); after 3 the answer is filled in and the game moves on. The 🔊 button reads the
question aloud.

**Unlocking.** Clearing **Level 5** of a game unlocks the next game. Clearing **Level 10** opens that
game's Endless mode: puzzles keep coming and keep getting harder, 3 hearts, one lost per wrong
answer, and a best score is kept. The games page only ever shows the games that are unlocked plus one
locked card showing what it takes to open the next one, so the child is never facing ten choices.

**Difficulty inside a level.** Puzzles get harder across the 8 questions of a round, and Endless mode
keeps pushing past Level 10 by growing the numbers.

---

## Game 1 — Brick Pyramids 🧱

A pyramid of Lego bricks where every brick is **the two bricks under it added together**. Some bricks
are blank. Tap a blank brick, type the number, press ✓.

Going up the pyramid is addition. Going down is subtraction (`5 + ? = 12`), which is where the real
thinking starts: the child has to find a brick he *can* work out, then use it to unlock the next one.

| Level | Name | What it adds |
|---|---|---|
| 1 | First Pyramid | 3 rows, small numbers, blanks only above the bottom |
| 2 | Bigger Bricks | same shape, two-digit sums |
| 3 | Missing Pieces | blanks in the bottom row — subtraction |
| 4 | Four Floors | taller pyramid, blanks anywhere |
| 5 | Tens Tower | two-digit bricks, totals in the hundreds |
| 6 | Brick Detective | several bottom bricks missing; needs a chain of deductions |
| 7 | Five Floors | 15 bricks, up to 7 of them blank |
| 8 | Hundreds Heights | three-digit adding and subtracting |
| 9 | Times Tower | the rule changes to **multiply** |
| 10 | Mystery Middle | only the top and the outside bricks are shown |

**Level 10 is the interesting one.** The middle bottom brick can't be worked out one step at a time —
it gets counted twice (or three times) on the way up, so it is really the equation
`a + 2b + c = top`. The child guesses, and the game answers with what the top *would* have been and
whether that is too big or too small, filling in the ghost numbers so he can see the effect. Two
guesses are free, so guess-and-check is a legitimate strategy, not a punished one.

## Game 2 — Pattern Machine ⚙️

A machine prints a row of numbers that follow a secret rule, with one (or two) missing. Find the
rule, type the missing number. After it's solved the machine shows its rule, and the 💡 hint reveals
the jumps between the numbers.

| Level | Name | Patterns |
|---|---|---|
| 1 | Counting Machine | +1, +2, +5, +10 |
| 2 | Jump Machine | bigger steps, and counting down |
| 3 | Missing Middle | the gap is in the middle of the row |
| 4 | Big Jumps | +25, +50, +99, +101, +250 |
| 5 | Doubler | ×2, ×3, ×5, ×10, halving |
| 6 | Growing Gaps | jumps that grow: square numbers, triangle numbers, odd-number jumps |
| 7 | Two-Step | two rules taking turns (+7 −2), "double it and add 1" |
| 8 | Fibonacci Factory | each number is the two (or three) before it added together |
| 9 | Zipper | two patterns zipped together, prime numbers, cube numbers, powers of 2 |
| 10 | Mastermind | everything mixed, two numbers missing |

## Game 3 — Googol Zoom 🚀

Big-number questions. Every right answer zooms a rocket further out — from the child's own height
past Mount Everest, Earth, the Sun, the galaxy, the edge of the visible universe, the number of atoms
in it, and finally to a googol and a googolplex.

The mathematical spine is that **multiplying powers of ten means adding their zeros** and dividing
means taking zeros away — which is exactly what exponents are.

| Level | Name | Content |
|---|---|---|
| 1 | Zero Counter | counting zeros, ×10, 999 + 1 |
| 2 | Zero Smash | 1,000 × 10,000 — add the zeros; and how adding differs from multiplying |
| 3 | Brain Teasers | digits vs zeros, "1,000 thousands or 1 million?", how long to count to a billion, how many 1 cm bricks in a 1 km tower |
| 4 | Front Digits | 30 × 200: multiply the fronts, then add the zeros |
| 5 | Power Code | 10³ notation; 10³ × 10⁴ = 10⁷ |
| 6 | Giant Names | billion, trillion, quadrillion, quintillion, and multiplying them |
| 7 | Zero Chop | dividing; how many thousands make a million |
| 8 | Power Towers | (10⁶)³, a million × a million × a million |
| 9 | Googol! | 10¹⁰⁰; googol × googol = 1 with 200 zeros; a googol beats the atoms in the universe |
| 10 | Googolplex | 1 with a *googol* zeros; googolplex × googol; which is bigger |

Answers that are too big to write are drawn as Lego plates of 100 zeros — a googol is one plate, a
googol squared is two.

## Game 4 — Brick Fit 🧩

Spatial reasoning, which is the aptitude a Lego builder already has and school almost never trains.
Some answers are typed; others are picked from pictures.

| Level | Name | What it asks |
|---|---|---|
| 1 | Stud Counter | how many studs on a plate — multiplication as an array |
| 2 | Split the Plate | an L-shaped plate: split it into two rectangles (the distributive law, in bricks) |
| 3 | Brick Towers | a 3D build: count every brick, including the ones inside |
| 4 | Hidden Bricks | towers of different heights; how many bricks are hidden underneath the tops |
| 5 | Same or Turned? | which piece is the same shape turned around — with a mirror image as the trap |
| 6 | Fill the Gap | which piece drops exactly into the hole in the plate |
| 7 | Mirror | tap out the mirror image of a shape across a line |
| 8 | Bird's Eye | what the build looks like from straight above; how many bricks to fill it into a solid box |
| 9 | Box Folding | which flat piece of six squares folds up into a cube |
| 10 | Master Builder | all of it mixed together |

The cube-net question uses a real folding simulation rather than a list: of the 216 six-square shapes,
it finds exactly the 11 that fold into a cube — so the wrong answers are genuinely wrong.

## Game 5 — Take-Away 🤖

A two-player take-away game (the Nim family) against a robot. Tap the bricks you want, press TAKE,
and whoever takes the last brick wins. Every level has a **secret rule** that wins every time, and
from Level 3 the robot plays perfectly — so the only way to win is to find the rule.

This is the one game in the set that is really about proof. "Leave a multiple of 4" is a theorem, and
the child tests it by never losing again. A win only counts as perfect if he never once handed the
robot a winning position, so the star rating measures the strategy rather than the outcome. After a
loss, the game shows the exact move where he gave it away: *you left 7 — leaving 8 would have won.*

| Level | Name | The game | The secret |
|---|---|---|---|
| 1 | Last Brick | take 1–3, robot plays badly | — |
| 2 | Robot Wakes Up | take 1–3, robot half-decent | — |
| 3 | Secret of Four | take 1–3, robot perfect | leave a multiple of 4 |
| 4 | New Limits | take up to 2, 4 or 5 | leave a multiple of (biggest take + 1) |
| 5 | Backwards | take 1–3, last brick **loses** | leave 1, 5, 9, 13… |
| 6 | Odd Jumps | take 1, 3 or 4 — never 2 | traps are 2, 7, 9, 14, 16… (repeats every 7) |
| 7 | Two Piles | any number from one pile | make the piles equal, then copy the robot |
| 8 | Odd One Out | three piles, two of them equal | take the whole odd pile |
| 9 | Three Piles | three piles, any size | break piles into 4s, 2s and 1s; leave an even number of each |
| 10 | The Golden Game | take from one pile, or the same from both | traps 1&2, 3&5, 4&7, 6&10 — the gaps grow by 1 (this is the golden ratio again) |

Hints are deliberately Socratic: the first tap asks a question, the second narrows it, and only the
third states the rule. The rule is also shown on the level-complete screen once the level is cleared.

## Game 6 — Gear Lab ⚙️

Technic gear ratios. Gears push each other tooth by tooth, so a big gear driving a small one spins it
faster, and a small gear driving a big one makes it slower — but stronger.

| Level | What it asks |
|---|---|
| 1–2 | the 24-tooth gear turns 3 times — how many turns is that for the 8-tooth one, and backwards |
| 3–4 | which way does the last gear turn, and what an **idler** in the middle does (nothing, to the speed) |
| 5 | which pair spins fastest: big driving small |
| 6 | two-stage trains, where the slowing-down **multiplies** |
| 7 | the gear has an unknown number of teeth — work it out from the turns |
| 8 | worm gears: one tooth per turn, the biggest gear-down there is |
| 9 | speed and strength: whatever you lose in one you gain in the other |
| 10 | design the train yourself to get the speed you want |

Once the answer is in, the gears spin at the correct relative speeds.

## Game 7 — Mystery Machine 🎛️

A function machine. Type a number, press TEST, and see what comes out. Test as many numbers as you
like, and when you think you know the rule, press **I know the rule!** — the machine then asks for
two predictions in a row. Both right and the rule is cracked.

This replaces "guess the rule I'm thinking of" with real hypothesis-testing: the child controls the
experiments, and the claim is only accepted when it predicts. Machines run from `+7` through
`×3 − 2`, `x × x`, backwards machines (you see the output, find the input), two-number machines,
chains of two machines, and tricky ones that count digits or ignore the input completely. Level 9
gives a finished test sheet and asks which rule fits **every** line.

## Game 8 — Target Builder 🎯

Countdown, for a six-year-old. Tap a number, tap an operation, tap another number — they join into
one new number. Keep going until you make the target. Numbers can be used once, not every number has
to be used, and **UNDO costs nothing**.

Levels move from three numbers and + only, to six numbers with 25/50/75/100 and a three-digit target.
Rounds here are **5 puzzles** rather than 8, because one puzzle can take ten minutes — which is the
point: this is the game that rewards sitting with a problem. Hints escalate: which two numbers to
start with, then the first step, then a full solution.

## Game 9 — How Many Ways 🔢

Counting without listing: the product rule (2 big bricks × 3 small ones = 6 towers), paths on a grid
going only right and down (the numbers are Pascal's triangle — the same rule as Brick Pyramids),
handshakes, arrangements, choosing teams, climbing stairs 1 or 2 at a time (Fibonacci again), flags
with no two stripes alike, two-dice totals, and squares hidden inside squares.

## Game 10 — Balance Scale ⚖️

Algebra with a mystery box. The two pans always weigh the same; find what's in the box. The one trick
behind all of it: **whatever you do to one pan, do to the other**.

| Level | What it asks |
|---|---|
| 1–2 | `? + 17 = 50`, and take-aways |
| 3–5 | `4 × ? = 28`, then two-step: `3 × ? + 7 = 37` |
| 6 | several identical boxes on one pan |
| 7 | boxes on **both** pans — take the same off each side |
| 8–9 | a box **and** a star, with two clues (add the clues and the stars cancel; or swap one into the other) |
| 10 | everything mixed — this is simultaneous equations, in pictures |

## Game 11 — Prime Factory 🏭

Multiples, sharing with remainders, how many rectangles a number can make (its factor pairs), prime
or not, factor trees, full prime factorisation, smallest-common and biggest-common numbers, and a
hands-on **sieve of Eratosthenes** where crossing out the multiples makes the primes appear.

## Game 12 — Binary Lights 💡

Lights worth 1, 2, 4, 8, 16, 32. Read the lights, make a number by switching them on, add one and
watch the lights roll over, work out how many numbers a row of lights can make, discover that sliding
everything one place left **doubles** it, and read 1s and 0s the way a computer writes them. Level 10
links it back to Take-Away: break each pile into 4s, 2s and 1s and count how many of each.

## Game 13 — Below Zero 🌡️

The number line past zero, on a thermometer, a number line and a lift going down into the basement.
Counting down past zero, temperature drops, distances from −6 to 4, adding and subtracting into the
negatives, which of two cold numbers is colder, and the number halfway between.

## Game 14 — Fraction Bricks 🍕

Fractions as bricks cut into equal pieces: naming what's shaded, equivalent fractions, a fraction
**of** a pile of bricks, comparing (a third beats a quarter), adding same-size pieces, how many
eighths are in 3 whole bricks, and finally adding halves to quarters.

---

## The games page

- **Math pictures.** Four pictures drawn in code — a Fibonacci spiral, a sunflower's seed spiral,
  Pascal's triangle with the odd numbers colored, and a Sierpiński triangle. Tapping one gives a
  short explanation and a question with a "Show answer" button. Pascal's triangle is deliberately the
  same rule as Brick Pyramids, upside down, and its odd numbers are the Sierpiński triangle.
- **Narration.** The 🗣️ button turns narration on and off, on the games page and inside every game.
  With it off nothing is read aloud automatically, but tapping 🔊 Read it still reads a question — for
  a child who can't read yet, or a grown-up who wants the room quiet.
- **Grown-ups panel.** Press and hold the ⚙︎ at the bottom of the games page for about a second:
  open all games and levels, sound effects, narration, which voice is being used (with a test
  button), a progress table, the roadmap, and a reset.

---

## Ideas for later

All fourteen games are built. Natural next steps, if he wants more:

- **Clock Math** — remainders and modular arithmetic ("if it's 9 o'clock, what time is it 100 hours
  later?"), which is also the pattern behind Take-Away Level 6.
- **Decimals and Money** — tenths and hundredths, following on from Fraction Bricks.
- **Measure It** — length, area and volume with bricks; perimeter vs area.
- **Chance** — dice and spinners, following on from How Many Ways Level 8.
- **Code Breaker** — simple ciphers, which turn letters into arithmetic.
- **Two-player mode for Take-Away** — the robot steps aside so he can beat a grown-up instead.

---

## Adding a game

Each game page is the same shared engine (level map, rounds, keypad, stars, sounds, narration) plus
one game module at the bottom of the file. A new game supplies a list of 10 levels and a
`make(level, puzzleIndex, boost)` function that returns a puzzle: some HTML with `data-blank` slots
(or a list of multiple-choice answers), the answers, a hint, and what to reveal once it's solved.
Adding it to the games page means one more entry in `CATALOG` (id, file, and which level of which
game unlocks it) and one entry in `LOOK` (color, description, icon).

Games that aren't question-and-answer — a board game, a tap-grid — set `custom: true` and drive the
round themselves through a small API (`mistake()`, `msg()`, `controls()`, `finish({win, reveal})`),
which is how Take-Away and the Mirror level of Brick Fit work.
