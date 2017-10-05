# Brandes-algorithm
Concurent implemenation of brandes algorithm. In simple words it allows to deiscover the most important nodes in graphs, for
example to find the most important influencers in social network. The code is capable to use power of all threads avaiable in computer.

**Node betweenness centrality: the definition**

Betweenness centrality for a node v is defined in terms of the proportion of
shortest paths that go through v. Specifically:
1. Assume a directed, unweighted, connected graph G =< V, E >.
2. Define σ(s, t) as the number of shortest paths between nodes s and t.
3. Define σ(s, t|v) as the number of shortest paths between nodes s and t
that pass through v.
4. CB(v), the betweenness centrality of v is defined as:
CB(v) = X
s,t∈V
σ(s, t|v)
σ(s, t)
If s = t, then σ(s, t) = 1. If v ∈ s, t, then σ(s, t|v) = 0.
Brandes’ algorithm is for the case where we want to calculate this efficiently for
every node.

*taken from : [http://www.cl.cam.ac.uk/teaching/1617/MLRD/handbook/brandes.pdf]*
