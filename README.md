# Isomorphism

Prove that if two graphs $A$ and $B$ are isomorphic they do *not* have to
be completely connected. I have started with the formal definition of
isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

Proof w/ Markdown Notation:
----------------------------
# Case 1: Two Isomorphic Graphs A & B are fully connected.
This is trivially True; as two isomorphic graphs A and B are fully connected and retain isomorphism {Defintion of Isomorphism}

# Case 2: At least A or B is not fully connected, given A and B are Isomorphic Graphs.
let's assume A is not fully connected. Since A & B are isomorphic there exists a bijection $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ if  $(f(u),f(v)) \in E_2$. {definition of Isomorphism}

As is not fully connected there exists at least one pair of vertices $(u,v) \in V_1$ that $(u,v)\notin E_1$, meaning they have no adjacency and thus are not connected. Therefore, their corresponding vertices $f(u),f(v) \in V_2$ must $(f(u),f(v))\notin E_2$ as the bijection $f$ preserves said relation.

Subsequently, B is not fully connected as it contains at least one set of vertices, preserved by the bijection $f$ such that $f(u),f(v) \in V_2$ AND $(f(u),f(v))\notin E_2$. {definition of Isomorphism} {definition of fully connected}

as a result, two isomorphic graphs A and B are both not fully connected, yet isomorphic.

# Conclusion:
"case 1" proves trivially that two fully connected graphs that are Isomorphic retain said Isomorphism. "case 2" proves two isomorphic graphs A & B are mutually not fully connected, yet remain isomorphic. Therefore, two isomorphic graphs A and B don't have to be fully connected
