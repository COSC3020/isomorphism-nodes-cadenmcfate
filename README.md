[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/AtNXzL3S)
# Isomorphism

Prove that if two graphs $A$ and $B$ do not have the same number of nodes, they
cannot be isomorphic. I have started with the formal definition of isomorphism
below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

## Answer

Let $A = (V_A , E_A)$ and $B = (V_B, E_B)$ be two graphs. We want to show that if $|V_A| \neq |V_B|$, $A$ and $B$ cannot be isomorphic.

Case 1: Assume $|V_A| < |V_B|$:

We wish to find a bijection from $V_A$ to $V_B$ that satisfies the isomorphic properties. We see this is not possible. Since the domain has less elements than the codomain, the function will at most be 1-1 or onto, but not both. In order to have a 1-1 function, 1 or more elements of $V_B$ will not have any mappings; the function won't be onto. And in order to have an onto function, 1 or more elements of $V_A$ will map to multiple items of $V_B$, making it no longer 1-1. 

Case 2: Assume $|V_A| > |V_B|$:

In this case we can strictly say that the function cannot be 1-1. Attempting to do so would leave out 1 or more elements of the domain, meaning we no longer have an actual function.

Therefore, if two graphs do not have the same number of nodes, they cannot be isomorphic.
