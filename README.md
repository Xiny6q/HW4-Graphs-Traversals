Download link :https://programming.engineering/product/hw4-graphs-traversals/


# HW4-Graphs-Traversals
HW4: Graphs, Traversals
Q1. Given an undirected graph with 10 vertices but 45 edges, which of the following will be true? Select all that apply.

Every node will have at least one neighbor

The graph will have duplicate labels

An Adjacency List would be more space-efficient to represent this graph vs. a Matrix

The graph is GUARANTEED to have a cycle in it

None of the above

A and D are true.

Q2. There are N cities, with M roads, where each road connects a pair of cities. You are given city x. We want to see if every city has a direct road leading to x. Return true if this condition is met, and false otherwise.

If we represent this as a graph problem, what are the nodes and edges?

The nodes are the cities and the roads are the edges

Is this a directed or undirected graph? – Please consider the situation between two cities in the real world. The question is not about two places in a city.

Undirected

Given an adjacency matrix for this graph, describe using words how you would find the answer to this problem. You do not have to write code.

Check the row “x” in the matrix and if every column except for “x” has a value of 1 then every city has a direct road leading to x.

Given an adjacency list for this graph, describe using words how you would find the answer to this problem. You do not have to write code.

Traverse through the list of entry “x” in the adjacency list. If all other cities are listed in the adjacency list then it is directly connected to all the cities.

Q3. Given the graph below, answer the following questions.


Represent this graph as an adjacency list.

0={}

1 = {0,2,4}

2={0}

3={0}

4={3}

Represent this graph as an adjacency matrix.

0

1

2

3

4

0

0

0

0

0

0

1

1

0

1

0

1

2

1

0

0

0

0

3

1

0

0

0

0

4

0

0

0

1

0

Write your Java code(submit a .java file) to implement the DFS for graph traversal using the adjacency matrix (either recursive or iterative).

For the test case, you can directly use the above example. And you should call the DFS function several times with different starting points to show the different traversal orders.

DFS(graph, 0); // one possible output likes 0

DFS(graph, 1); // one possible output likes 1 0 2 4 3

DFS(graph, 2); // …

DFS(graph, 3); // …

DFS(graph, 4); // …

(DONE)
