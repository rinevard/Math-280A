# Homework 2

## Problem 1
Let $\Omega = \{1, 2, 3, 4\}$, and set $S = \{\emptyset, \{1\}, \{2\}, \{3, 4\}, \Omega\}$.

(a) Prove that $S$ is a semi-algebra. \
(b) Define $\chi: S \to \mathbb{R}$ as follows:

$$\chi(\emptyset) = 0, \chi(\{1\}) = \chi(\{2\}) = \chi(\{3, 4\}) = 1, \chi(\Omega) = 4.$$

Show that $\chi$ is "pairwise" additive: $\chi(A \cup B) = \chi(A) + \chi(B)$ whenever $A, B,$ and $A \cup B$ are all in $S$. Show also that $\chi$ is not additive over all finite disjoint unions.

(This shows it is important, when dealing with semi-algebras and other classes not closed under finite union, to spell out the full statement of "finite additivity" in all proofs.)

## Problem 2
(Exercise 4.12 in Driver) Let $\Omega_1$ and $\Omega_2$ be sets, and let $\mathcal{A}_1 \subseteq 2^{\Omega_1}$ and $\mathcal{A}_2 \subseteq 2^{\Omega_2}$ be semi-algebras. Show that

$$S = \mathcal{A}_1 \times \mathcal{A}_2 = \{A_1 \times A_2 : A_1 \in \mathcal{A}_1, A_2 \in \mathcal{A}_2\} \subseteq 2^{\Omega_1 \times \Omega_2}$$

is a semi-algebra.

## Problem 3
(Exercise 4.3 in Driver) Let $A_n, B_n \subseteq \Omega$ for $n \in \mathbb{N}$. Show that

$$\left(\bigcup_{n=1}^{\infty} A_n\right) \setminus \left(\bigcup_{n=1}^{\infty} B_n\right) \subseteq \bigcup_{n=1}^{\infty}(A_n \setminus B_n).$$

Use this to show that

$$\left(\bigcup_{n=1}^{\infty} A_n\right) \triangle \left(\bigcup_{n=1}^{\infty} B_n\right) \subseteq \bigcup_{n=1}^{\infty}(A_n \triangle B_n).$$

## Problem 4
(Exercise 4.4 in Driver) Let $A, B, C \subseteq \Omega$. Recall that the **symmetric difference** of sets is $A \triangle B = (A \cap B^c) \cup (B \cap A^c)$.

(a) Show that $A \cap C^c \subseteq (A \cap B^c) \cup (B \cap C^c)$.

(b) Use part (a) to show that

$$A \triangle C \subseteq (A \triangle B) \cup (B \triangle C).$$

(c) Now, let $\nu: 2^\Omega \to [0, \infty)$ be an outer measure. Show that the function $d: 2^\Omega \times 2^\Omega \to [0, \infty)$ defined by $d(A, B) = \nu(A \triangle B)$ satisfies the **triangle inequality**:

$$d(A, C) \leq d(A, B) + d(B, C).$$

## Problem 5
Let $\mathcal{A}$ be a field over $\Omega$, and let $\mathbb{P}$ be a probability measure on $(\Omega, \sigma(\mathcal{A}))$. Let $B \in \sigma(\mathcal{A})$. Prove that for any $\epsilon > 0$, there is a set $A \in \mathcal{A}$ such that $\mathbb{P}(A \triangle B) < \epsilon$. I.e. $\mathcal{A}$ is "dense" in $\sigma(\mathcal{A})$. \
[Hint: show that the collection of all sets $B$ satisfying this property is a $\sigma$-field.]