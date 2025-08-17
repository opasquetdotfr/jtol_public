<img width="1040" height="494" alt="delaunay_tree" src="https://github.com/user-attachments/assets/948a5918-ca98-4b0b-8e9a-62f8b1cf6cc1" />

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

<img width="600" height="516" alt="04_demo_jtol bach_ ratio_" src="https://github.com/user-attachments/assets/c7cf1620-33e6-4b71-82d3-e8942a792651" />

---

#### jtol.bach.henon

`jtol.bach.henon` is one of the available generators. It performs the [Henon map](en.wikipedia.org), a non‑linear two‑dimensional discrete deterministic dynamical system.

For most generators, each parameter can be a [scalar](en.wikipedia.org), a [vector](en.wikipedia.org), or a [tree](en.wikipedia.org). This allows cell-by-cell and step-by-step control for the generated [forms](en.wikipedia.org).

<img width="300" height="241" alt="jtol_bach_henon-300x241" src="https://github.com/user-attachments/assets/1ad38bd8-2f8a-4565-8b62-0de9e8e8630d" />

---

#### jtol.bach.play

`jtol.bach.play` converts ratios from `jtol.bach2score` into millisecond timings and outputs corresponding time-delayed bangs when a `play` message is received.

<img width="600" height="364" alt="02_demo_jtol bach_ play_" src="https://github.com/user-attachments/assets/80dd4303-6c7f-44b4-9226-827d355b8d9b" />

---

#### jtol.bach.dur

`jtol.bach.dur` retrieves all durations of a jtol tree.

<img width="600" height="414" alt="03_demo_jtol bach_ dur_" src="https://github.com/user-attachments/assets/7a493c37-4835-4aee-8224-65ec8f41fd44" />

---

#### jtol.bach2score

`jtol.bach2score` gathers a time tree representation for bach.score. The time signature is calculated from the incoming tree and the note value.

<img width="600" height="536" alt="01_demo_jtol bach2score" src="https://github.com/user-attachments/assets/6a2f9254-727e-4c93-856f-0bc361797401" />

---

#### jtol.bach.reduce

`jtol.bach.reduce` reduces the depth of trees. For example:

<img width="600" height="532" alt="14_demo_jtol bach_ reduce" src="https://github.com/user-attachments/assets/e4338091-884a-4614-a99b-2d447a7cb7ec" />
