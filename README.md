# Kruskal-s-Algorithm
This is a Kruskal’s Algorithm with C.


The Kruskal's algorithm performs a Union-Find operation by comparing the set of two vertices that connect the edges by sequentially drawing from the smallest edges.

Kruskal’s Algorithm Pseudocode:

Kruskal(G, w)
{
	A = empty set;
	for each v ⊆ G.V
		Make_set(v)
	sort G.E by increasing edge weight w
	for each edge (u, v) ⊆ G.E (in sorted order)
		if Find_set(u) != Find_set(v)
		A = A U {{u,v}};
		Union(u, v);
	return A
}
