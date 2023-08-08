# Avg-Linear-Time-Diameter-algorithm
Presenting linear O(M) Diamter finding algorithm with worst case O(m * n). This is simply a C++ implementation of this iFUB algorithm.

<h2>iFUB Algorithm</h2>
nput: A graph G, a node u, a lower bound l for the diameter, and an integer k
Output: A value M such that D − M ≤ k
i ← ecc(u);
lb ← max{ecc(u), l};
ub ← 2ecc(u);
while ub − lb > k do
if max{lb, Bi(u)} > 2(i − 1) then
return max{lb, Bi(u)};
else
lb ← max{lb, Bi(u)};
ub ← 2(i − 1);
end
i ← i − 1;
end
return lb;

# NOT COMPLETED
Accept help from Anyone. Simply push it.

# Cite
Pilu Crescenzi, Roberto Grossi, Michel Habib, Leonardo Lanzi, Andrea Marino,
On computing the diameter of real-world undirected graphs,
Theoretical Computer Science,
Volume 514,
2013,
Pages 84-95,
ISSN 0304-3975,
https://doi.org/10.1016/j.tcs.2012.09.018.
(https://www.sciencedirect.com/science/article/pii/S0304397512008687)
Abstract: We propose a new algorithm for the classical problem of computing the diameter of undirected unweighted graphs, namely, the maximum distance among all the pairs of nodes, where the distance of a pair of nodes is the number of edges contained in the shortest path connecting these two nodes. Although its worst-case complexity is O(nm) time, where n is the number of nodes and m is the number of edges of the graph, we experimentally show that our algorithm works in O(m) time in practice, requiring few breadth-first searches to complete its task on almost 200 real-world graphs.
Keywords: Breadth-first search; Diameter; Complex network; Experimental analysis
