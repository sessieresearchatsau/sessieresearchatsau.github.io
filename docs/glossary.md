### 📘 Glossary of Terms and Concepts

| Term                          | Explanation |
|-------------------------------|-------------|
| **Sequential Substitution System (SSS)** | A system where a string evolves step-by-step by applying substitution rules in a fixed left-to-right order. |
| **Sessie** | A nickname for a Sequential Substitution System (SSS). |
| **State String**              | The current configuration of characters representing the system’s state at a given time. |
| **Substitution Rule**         | A transformation that replaces one substring with another, defining the system’s behavior. |
| **Event**                     | A single application of a rule that modifies the state string by creating or destroying characters. |
| **Causal Connection**         | A relationship where one event creates a character that another later destroys. |
| **Causal Network**            | A graph of events linked by causal connections, representing the flow of information or influence. |
| **Toy Universe**              | A metaphor for the evolving state string governed by substitution rules—used to explore emergent behavior. |
| **Alphabet**                  | The set of characters used in the state string; often unbounded. |
| **Insertion Rule**            | A rule where the target is the empty string, allowing characters to be added. |
| **Deletion Rule**             | A rule where the replacement is the empty string, allowing characters to be removed. |
| **Multi-way Substitution System** | A variant where all applicable rules are applied simultaneously at all positions, generating multiple outcomes. |
| **Generalized Substitution System** | A superset that includes both sequential and multi-way substitution systems. |
| **Evolution**                 | The sequence of state strings generated over time as the system progresses. |
| **Rule Priority**             | The order in which rules are attempted—earlier rules take precedence. |
| **Leftmost Application**      | When a rule can be applied in multiple places, it is applied at the first (leftmost) valid position. |
| **Emergent Complexity**       | The phenomenon where simple rules lead to intricate and unpredictable behavior. |
| **Dimensional Extension**     | A theoretical idea of extending the 1D state string to 2D or higher dimensions, enabling block-based substitutions. |
| **Spring-Wrapped State**      | A speculative model where the state string wraps like a coil, enabling 2D pattern matching and insertion. |
| **Simple Program**            | A system defined by minimal rules that nonetheless produces rich, complex behavior. |
| **Cellular Automaton**        | A related concept where a grid of cells evolves based on local rules—used for comparison with SSSs. |
| **Turing Machine**            | A computational model with a tape and a head, used to illustrate how SSSs differ in structure and behavior. |
| **Enumeration**               | A systematic listing of all strings, rulesets, or configurations, often used to prove countability or explore all cases. |
| **Diagonal Enumeration**      | A method of listing elements (e.g., rational numbers) by traversing diagonals in a grid—used as a metaphor for rule indexing. |
| **Rank/Unrank Functions**     | Functions that map between elements and their position in an enumeration, enabling reversible indexing. |
| **Hyperbinary Function**      | A recursive function used to generate sequences for rational enumeration and causal indexing. |
| **Calkin–Wilf Tree**          | A binary tree that enumerates all reduced positive rational numbers, used as a model for indexing. |
| **Stern–Brocot Tree**         | A tree structure that enumerates all positive rational numbers without repetition, related to the Calkin–Wilf tree. |
| **Weight of a String**        | The sum of character weights (e.g., A=1, B=2, …), used to order strings in enumeration. |
| **Composition**               | A way of expressing a string’s structure as a sequence of weights, often used in ranking algorithms. |
| **Dimensionality Test**       | A method for identifying the dimension of a causal network by analyzing nth differences in event indices. |
| **Difference Table**          | A table of successive differences used to detect polynomial or exponential growth patterns. |
| **Exponential Network**       | A causal network where node growth follows exponential patterns, never yielding constant difference rows. |
| **Fractional Dimension**      | A concept where the difference table doesn’t yield a constant row, but fluctuates—suggesting non-integer dimensionality. |
| **Macrotime**                 | A coarse-grained view of time in the causal network, often observer-dependent. |
| **Microtime**                 | The fine-grained, local time flow represented by directed edges in the causal network. |
| **Node-Origin Inaccessibility** | A situation where certain nodes cannot be reached from the origin, raising questions about causality and dimensionality. |
| **Edge Effects**              | Unique behaviors or structural features at the boundaries of a causal network. |
| **Dimensional Ambiguity**     | When different tests yield conflicting results about the network’s dimensionality. |
| **Tensor Character**          | A speculative idea that node density in 2D may reflect properties of a higher-dimensional space. |
| **Conformational Transformation** | A metaphor from chemistry suggesting that networks may stretch, bend, or oscillate while preserving causal structure. |
| **A New Kind of Science (NKS)** | A research approach by Stephen Wolfram that studies how simple computational rules, when systematically explored, yield complex behavior and reveal deep insights into math, physics, and natural systems. |
| **Mining the Computational Universe** | The NKS strategy of exploring all simple rules to discover emergent behavior. |

---
