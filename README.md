# jtol

🔴 JTOL is currently private. Please contact me if interested.

# Jtol is a Max/MSP library for rhythm and pattern generation using a tree structure.

Jtol is built and used by jt rinker and olivier pasquet. It is a library dedicated to real-time pattern generation and can be applied to architectural design, music, dance; and everything requiring constructed evolution in space and time. It deals with multi-scaling and multi-dimensions where rhythm is considered to be a skeleton onto which everything else is attached (pitches, params…).  Jtol was first programmed in python in max with the help of bertrand nouvel. It gathered data structures similar to the jitter library but with a nested architecture. A newer version is now using the bach library and still runs in max. It has nevertheless been programmed in order to always be able to easily get rid of the bach library. It is inspired by libraries like athenaCL, numpy, scipy, abjad, pyevolve, pwgl and open music. Some purely generative music devices will soon come for max for live.

For Max 8.2.2 and bach 0.8.1 beta.

http://www.opasquet.fr
https://cycling74.com/downloads/
http://www.bachproject.net/download

---

### Here are some possible interests for jtol:

- ENP-like notation in Max, nested tree system for rhythm  
- Beat repetitions, loop-based generators  
- Braid theory, tessellation  
- Cellular automata and multi-agent systems  
- Chaos  
- Sieves  
- Permutative, serial functions  
- Multi-order Markov chains  
- Multi-set  
- Quantization, interpolation and extrapolation  
- Pitch functions  
- Genetic algorithms

---

### Examples

#### jtol.bach.ratio

`jtol.bach.ratio` gives rational values from a tree representation. Inspired by [ENP notation](www2.siba.fi), it is very pretty and convenient for [rhythmic musical structures](en.wikipedia.org) where durations are filled in rational ways. Ratios are nested with parentheses to create a multilevel tree.

Each ratio before a new parenthesis level is the total duration for what is inside that parenthesis. For example, simple musical tuplets:

- `( 1 ( 1 1 1 ) )` → `( 1/3 1/3 1/3 )` → `( 0.333 0.333 0.333 )` (Σ = 1)  
- `( 1 ( 1 1 ( 1 1 1 ) ) )` → `( 1/2 1/6 1/6 1/6 )` → `( 0.5 0.1667 0.1667 0.1667 )` (Σ = 1)

There's a close relation with spatial tessellations like [Voronoi](en.wikipedia.org), where the [Delaunay triangulation](en.wikipedia.org) is practical.

![Delaunay Triangulation – Olivier Pasquet – 2012](Image: delaunay triangulation - Olivier Pasquet - 2012)  
![jtol.bach.ratio – Olivier Pasquet – 2012](Image: jtol.bach.ratio - Olivier Pasquet - 2012)

---

#### jtol.bach.henon

`jtol.bach.henon` is one of the available generators. It performs the [Henon map](en.wikipedia.org), a non‑linear two‑dimensional discrete deterministic dynamical system.

For most generators, each parameter can be a [scalar](en.wikipedia.org), a [vector](en.wikipedia.org), or a [tree](en.wikipedia.org). This allows cell-by-cell and step-by-step control for the generated [forms](en.wikipedia.org).

![jtol.bach henon – Olivier Pasquet – 2012](Image: jtol.bach henon - Olivier Pasquet 2012)

---

#### jtol.bach.play

`jtol.bach.play` converts ratios from `jtol.bach2score` into millisecond timings and outputs corresponding time-delayed bangs when a `play` message is received.

![jtol.bach.play – Olivier Pasquet – 2012](Image: jtol.bach.play - Olivier Pasquet - 2012)

---

#### jtol.bach.dur

`jtol.bach.dur` retrieves all durations of a jtol tree.

![jtol.bach.dur – Olivier Pasquet](Image: jtol.bach.dur - Olivier Pasquet)

---

#### jtol.bach2score

`jtol.bach2score` gathers a time tree representation for bach.score. The time signature is calculated from the incoming tree and the note value.

![jtol.bach2score – Olivier Pasquet](Image: jtol.bach2score - Olivier Pasquet)

---

#### jtol.bach.reduce

`jtol.bach.reduce` reduces the depth of trees. For example:
