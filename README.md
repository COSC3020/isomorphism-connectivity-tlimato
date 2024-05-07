[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/QM7QGF1q)
# Isomorphism

Prove that if two graphs $A$ and $B$ are isomorphic they do *not* have to
be completely connected. I have started with the formal definition of
isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

## Proof
I just sat down and completely reworked the problem. I stared at my original work and read your feedback and then realized I am way overcomplicating this. Simply by using proof by counter example, we can prove that if two graphs are isomorphic, they don't have to be fully connected without generalizing that if one isomorphic graph is not fully connected then the other isn't fully connected either.

For a Graph to be complete, it must have an edge present between every pair of distinct vertices.

Given we are told we can assume the two graphs $A$ and $B$ are isomorphic, we can assume there exists a function $f: V_A \rightarrow V_B$ such that $(a,b) \in E_A$ if $(f(a),f(b)) \in E_B$. This function $f$ is a bijection, so it is one-to-one and onto for the Graphs $A$ and $B$.

### Proof by counter example.

- Let $A$ be a graph  with the following set of vertices: $V_A = (a,b)$ and no edges, meaning $E_A = \emptyset$.

- Let $B$ be a graph with the following set of vertices: $V_B = (u,v)$ and no edges, meaning $E_B = \emptyset$.

By definition, neither $A$ or $B$ are connected, as there are no edges between the discrete vertices at all.

Given we are told we can assume the two graphs $A$ and $B$ are isomorphic, we can assume there exists a bijjection function $f: V_A \rightarrow V_B$ such that $(a,b) \in E_A$ if $(f(a),f(b)) \in E_B$.

We can then validate that $A$ and $B$ are still isomorphic despite not being fully connected through validating the properties of $f$.

- we can simply define the following regarding the vertices, $f(a) = u$ and $f(b) = v$.

- Since there are no edges in the graph $A$ and there are no edges in $B$ neither are fully connected and yet the condition $(a,b) \in E_A$ if $(f(a),f(b)) \in E_B$ is trivially satisfied by the function $f$ and we can say that $A$ and $B$ are still isomorphic.
This conclusion clearly demonstrates that if two graphs are isomorphic they do not have to be fully connected.


## Citations

My Notes from the videos and the previous submission.
I looked over my submission for https://github.com/COSC3020/isomorphism-nodes-tlimato/pulls which is what inspired me to try a proof by contradiction.

General Disclaimer:
I use Github copilot to assist in writing code, It's built into my vs code install I use for Professional work and It's helpful in accelerating projects and avoiding syntax issues. I will make this clarification on other assignments as well.
