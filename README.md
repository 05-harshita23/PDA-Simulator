# Pushdown Automata (PDA) Simulator

An interactive, single-file web application for simulating and visualizing Nondeterministic Pushdown Automata (NPDA). 

This tool is designed for educational purposes, allowing users to build, step through, and visualize the execution of context-free languages (CFLs).

## Features
* **Interactive State Diagram:** Auto-generated, force-directed SVG graphs that highlight active states and transitions during execution.
* **Step-by-Step Execution:** Pause, step forward, and step backward through the simulation to watch the stack and input tape change in real-time.
* **Nondeterministic Computation Trees:** Automatically generates branching trees to visualize how the machine handles nondeterministic guesses.
* **Preset Library:** Includes built-in, classic examples of CFLs (e.g., $a^n b^n$, balanced parentheses, palindromes).
* **Custom Editor:** Build your own PDA using an intuitive transition table or bulk-import via JFLAP/Simple formats.
* **Zero Dependencies:** Built entirely in vanilla HTML, CSS, and JavaScript. No backend or package manager required.

## How to Run
Because this is a single-file application, no installation or local server is required.
1. Download or clone this repository.
2. Double-click the `index.html` file to open it in any modern web browser (Chrome, Firefox, Edge, Safari).
3. (Optional) You can view the live, hosted version of this project here: **[INSERT YOUR GITHUB PAGES LINK HERE]**

## Theoretical Foundation
This simulator strictly implements the formal 7-tuple definition of a Pushdown Automaton:
**M = (Q, Σ, Γ, δ, q₀, Z, F)**

* **Q**: Finite set of states
* **Σ**: Input alphabet
* **Γ**: Stack alphabet
* **δ**: Transition function
* **q₀**: Start state
* **Z**: Initial stack symbol
* **F**: Set of accept/final states

Acceptance in this simulator is defined by reaching a **final state** after the input string has been completely consumed.

## Tech Stack
* **HTML5:** Semantic structure and layout.
* **CSS3:** Custom dark-mode UI with glassmorphism and modern developer-tool aesthetics.
* **JavaScript (Vanilla):** Engine logic, DOM manipulation, SVG math generation, and nondeterministic pathfinding algorithms.
