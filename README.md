# Elementary Linear Algebra

<img src="./img/cover.png" width="200">

My study notes for the book "Elementary Linear Algebra" 1st edition (1964) by James R. Munkres.

- [Book's Contents](#books-contents)
- [Concept Map](#concept-map)
- [Minimum Route](#minimum-route)
- [A Nice-to-Have Theorem](#a-nice-to-have-theorem)
- [Selected Solutions](#selected-solutions)

## Book's Contents

| Chapter | Title                                     | Thoerem                      | Corollary |
| ------- | ----------------------------------------- | ---------------------------- | --------- |
| 1       | Vector Spaces                             |                              |           |
| 2       | Subspaces                                 | 2.1, 2.2                     |           |
| 3       | A Useful Theorem                          | 3.1                          |           |
| 4       | Linear Independence, Bases, and Dimension | 4.1, 4.3, 4.4, 4.5, 4.6      | 4.2       |
| 5       | Row Operations on Matrices                | 5.1, 5.2                     | 5.3       |
| 6       | Homogeneous Systems                       | 6.1, 6.2                     |           |
| 7       | The General System                        | 7.1, 7.4                     | 7.2, 7.3  |
| 8       | Determinants                              | 8.1, 8.2, 8.4, 8.5, 8,6, 8.7 | 8.3       |
| 9       | Function Spaces                           |                              |           |

## Concept Map

- Concept Map (Major Concepts + All Theorems and Corollaries) [`.mermaid`](./mermaid/ela.mermaid) [`.png`](./img/ela.png) [`.svg`](./img/ela.svg)

![](./img/ela.png)

1. *An arrow from box A to box B, i.e. `A --> B`, indicates that "A underlies B" or "A establishes B."*
2. *For brevity, in the case of transitive dependency, i.e. `A --> B --> C`, we will not draw an additional arrow from A to C, unless that relationship is crucial.*

## Minimum Route

- A Minimum Route to Corollary 7.3 (Column Rank Equals Row Rank) [`.mermaid`](./mermaid/min.mermaid) [`.png`](./img/min.png) [`.svg`](./img/min.svg)

![](./img/min.png)

1. *An arrow from box A to box B, i.e. `A --> B`, indicates that "A underlies B" or "A establishes B."*
2. *For brevity, in the case of transitive dependency, i.e. `A --> B --> C`, we will not draw an additional arrow from A to C, unless that relationship is crucial.*

## A Nice-to-Have Theorem

Theorem 4.4 says

> (Theorem 4.4) Let p be the dimension of W. Then any independent set of vectors of W consisting of p vectors necessarily spans W.

It's nice to have a "dual" theorem

> (Dual Theorem 4.4) Let p be the dimension of W. Then any spanning set of vectors of W consisting of p vectors are linearly independent.

***Proof*** &nbsp; Let $S = \lbrace\boldsymbol{a_1}, \dots, \boldsymbol{a_p}\rbrace$ be a spanning set of $W$. Suppose $S$ is not linearly independent, then by definition of linear independence, there must be some vector $\boldsymbol{a_k} \in S$ which can be expressed as a linear combination of other vectors in $S$. Then any vector in $W$, which can be expressed with vectors in spanning set $S$, can also be expressed without using $\boldsymbol{a_k}$. That is, $S\ \backslash\ \lbrace\boldsymbol{a_k}\rbrace$ is also a spanning set of $W$. This spanning set has $p - 1$ vectors. But by definition of dimension $p$, the largest linearly independent set in $W$ has $p$ vectors. This contradicts *Theorem 4.3*, which says any linearly independent sets can have no more vectors than do any spanning sets in a given subspace. Therefore, $S$ must be linearly independent. ∎

With the above theorems, we can conclude that given any two of the following three properties, we can readily obtain the third for a set of vectors -

1. is linearly independent
2. is spanning
3. has dimension number of vectors

## Selected Solutions

- See [`sol.md`](./markdown/sol.md)
