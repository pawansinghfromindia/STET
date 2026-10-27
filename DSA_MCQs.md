
## Data Structure and Algorithm

Q 1. The recurrence equation `T(n) = T(n/2) + T(n/3) + n` represents the time complexity of which algorithms paradigm?
- [x] A. Divide and Conquer
- [ ] B. Dynamic Programming
- [ ] C. Greedy Algorithms
- [ ] D. Backtracking

 <details>
   <summary> Solution </summary>

Application of **Dynamic programming**:
- `Floyd Warshall`
- `Bellman Ford` (Single source shortest path)
- `0-1 Knapsack` problem

Application of **Greedy Alogorithms**:
- `Prim's` for Minimum spanning tree
- `Kruskal's` for Minimum Spanning Tree
- `Dijstra's` for finding shortest path (Single source shortest path, problem arises here regarding -ve edge cycle)
- `Fractional Knapsack` Problem (which is 0-1 Knapsack problem solved in DP, this is version of that, can be solved using Grredy
  approach

Application of **Backtracking**:
- `N-Queen` Problem
- `Rat in a maze` problem
- `Graph Coloring` problem
 
 </details>
 <!-------------------------------------->

---

Q 2. In a threaded binary tree, the space required for thread is usually:
- [ ] A. greater than the space required for regular pointers
- [x] B. equal to the space required for regular pointers
- [ ] C. less than the space required for regular pointers
- [ ] D. Unpredicted

 <details>
   <summary> Solution </summary>

```
Normal Binary Tree:
                [  | 5 |  ]
                 /       \
  [ Null | 6 |  Null ]     [ Null | 9 |  Null ]

---------------------------------------------------

Threaded Binary Tree: Don't have Null, It is attached to their succesor and predecesor
                [  | 5 |  ]
                 /       \
  [ add of pre | 6 |  add of suc ]     [ Null | 9 |  Null ] 


```

 
 </details>
 <!-------------------------------------->

---

Q 3. In a B-Tree of order `m`, each internal node can have upto _______ children.
- [ ] A. `m-1`
- [x] B. `m`
- [ ] C. `2m-1`
- [ ] D. `2m`

 <details>
   <summary> Solution </summary>

```
4 order B Tree

max keys = m-1
min keys = (m-1)/2 = m/2 = m
```
 
 </details>
 <!-------------------------------------->

---

Q 4. In condtional asympotatic notation, "Θ(f(n)) if g(n)" indicates that the algorithm's complexity is both upper and lower
bounded by f(n) when:
- [ ] A. g(n) is a lower bound on f(n)
- [ ] B. g(n) is a upper bound on f(n)
- [x] C. g(n) is true
- [ ] D. g(n) is false

 <details>
   <summary> Solution </summary>

[Asympotatic notation](https://www.geeksforgeeks.org/dsa/types-of-asymptotic-notations-in-complexity-analysis-of-algorithms/)


```
Θ simply means -> lower boundary and upper boundary

Complexity will be always true bcuz we have upper and lower bound both functions are covering.
```
 
 </details>
 <!-------------------------------------->

---

Q 5. Separate chaining involves storing collided elements in separate data structures, typically in:
- [x] A. Linkedlists
- [ ] B. Arrays
- [ ] C. Stacks
- [ ] D. Queues

 <details>
   <summary> Solution </summary>

Hashing, In hashing we use a hash table where we need to store data like keys-values in a table.
This is done using a hash function.

Hash Function will generate a location and that location will hold the data by which searching become fast like
index based.

This can be done using ways:
1. Separate chaining: in hashtablem, by chaining linked list 
2. Open addressing
 
 </details>
 <!-------------------------------------->
 
---

Q 6. The Floyd-warshall algorithm is popular method for solving the All-pair Shortest Paths problem.
What is the time complexity of the Floyd Warshall for a graph with n-vertices?
- [ ] A. O(n)
- [ ] B. O(nlog)
- [ ] C. O(n^2)
- [x] D. O(n^3)

 <details>
   <summary> Solution </summary>

```
      A  B  C  D  E
  A [ 01 02 03 04 05 ]
  B [ 05 07 08 09 10 ]
  C [ 11 12 13 14 15 ]

n x (n^2) = n^3
```

[floyd-warshall-algorithm](https://www.geeksforgeeks.org/dsa/floyd-warshall-algorithm-dp-16/)

Time Complexity:
- We need 3 loops to implement the algorithm. Each loop has constant complexity. <br/>
Therefore, the time complexity is `O(n³)`. Here, n is the total no. of vertices in a graph.

Space Complexity:
- The space complexity of Floyd Warshall Algorithm is `O(n²)`.

Floyd Warshall Algorithm Applications
- To find the shortest path is a directed graph
- To find the transitive closure of directed graphs
- To find the Inversion of real matrices
- For testing whether an undirected graph is bipartite
 
 </details>
 <!-------------------------------------->

---

Q 7. A* search algorithms is based on?
- [ ] A. BFS
- [ ] B. DFS
- [ ] C. Uniform Cost Search
- [x] D. Best First Search

 <details>
   <summary> Solution </summary>

The A search algorithm* is fundamentally based on the best-first search method, 
specifically combining the strengths of Dijkstra’s algorithm (uniform-cost search) 
and greedy best-first search. 

It achieves this by using an evaluation function `f(n)=g(n)+h(n)`, which balances:
- g(n): The actual cost of the path from the start node to the current node (from Dijkstra's). 
- h(n): A heuristic estimate of the cost from the current node to the goal (from Greedy Best-First Search). 

This combination allows A* to efficiently find the shortest path in weighted graphs while 
maintaining completeness and optimality (provided the heuristic is admissible). 
 
 </details>
 <!-------------------------------------->

---

Q 8. In BFS, vertices are explored level by level, starting from the:
- [ ] A. Deepest level
- [x] B. Shallowest level(Root/first node) 
- [ ] C. Middle level
- [ ] D. Highest level degree

 <details>
   <summary> Solution </summary>

[BFS](https://www.scaler.com/topics/data-structures/breadth-first-search/)
 
 </details>
 <!-------------------------------------->

---

Q 9. Stack works on the principle of:
- [ ] A. Mid Element First
- [ ] B. First In First Out
- [x] C. Last In First Out
- [ ] D. Last in Last Out

 <details>
   <summary> Solution </summary>

[Stack](https://www.w3schools.com/dsa/dsa_data_stacks.php)
 
 </details>
 <!-------------------------------------->

---

Q 10. In the backtracking approach for the 8-Queens problems, once a feasible solution is found, the algorithm:
- [ ] A. Stop and return the solution
- [x] B. Continue searching for more solutions
- [ ] C. Iterates through all possibilities
- [ ] D. Rearranges the queens to optimize the solutions

 <details>
   <summary> Solution </summary>

```
Backtracking work is :
1. Backtracking uses DFS
2. It is backtracking job is to provide all the feasible solutions

Whereever dead-end encounter from there backtrack and then findout another solution.
```

[8-Queen problem](https://www.geeksforgeeks.org/dsa/8-queen-problem/)

[8-Queens problem](https://www.interviewbit.com/blog/8-queens-problem/)
 
 </details>
 <!-------------------------------------->

---

Q 11. Which sorting algorithms has a worst-case time complexity of O(n^2) in its basic form?
- [ ] A. Quick Sort
- [ ] B. Merge Sort
- [x] C. Insertion Sort
- [ ] D. Counting Sort

<details>
  <summary> Solution </summary>

```
Quick Sort -> O(n^2) But it is possible to make in O(n log n) by using randomised algo
Insertion Sort -> O(n^2)

Merge Sort -> O(n log n)
Counting sort -> O(n+k)
```

[Sorting Algorithms](https://www.geeksforgeeks.org/dsa/time-complexities-of-all-sorting-algorithms/)

</details>
<!----------------------------->

---

Q 12. Greedy Search strategy chooses the node for expansion in ________
- [ ] A. Shallowest
- [ ] B. Deepest
- [ ] C. The one close to the goal node
- [x] D. Minimum heuristic cost

<details>
  <summary> Solution </summary>

[Greedy Search Strategy](https://www.geeksforgeeks.org/dsa/greedy-algorithms/)

</details>
<!----------------------------->

---

Q 13. What is the primary goal of the backtracking approach in solving the Hamiltonian Cycle problem?
- [ ] A. To find a cycle with the fewest edges
- [ ] B. To find a cycle with the lowest weight
- [x] C. To find a cycle that visits every vertex exactly once
- [ ] D. To find a cycle with maximum number of edges

<details>
  <summary> Solution </summary>

```
Hamiltonian Graph:
- A graph where all of the vertices at least once covered, not necessaily edges but all vertices

Hamiltonian Cycle:
- when we start a node and ends with the same node, then it is Hamiltonian cycle
- A-B-C-D-A
```

[Hamiltonian Cycle](https://www.geeksforgeeks.org/dsa/hamiltonian-cycle/)

</details>
<!----------------------------->

---

Q 14. A threaded binary tree is a binary tree in which:
- [ ] A. Each node has two children
- [ ] B. Each node has at most one children
- [ ] C. Each node is connected to its parent
- [x] D. Each node has a thread connecting it to its predecessor or successor

<details>
  <summary> Solution </summary>

[Threaded Binary tree](https://www.naukri.com/code360/library/threaded-binary-trees)

</details>
<!----------------------------->

---

Q 15. Which data structure often results in a time-space trade off by usong extra memory to speed up operations?
- [ ] A. Arrays
- [ ] B. Linked lists
- [x] C. Hash tables
- [ ] D. Stacks

<details>
  <summary> Solution </summary>

[Hash Tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)

</details>
<!----------------------------->

---

Q 16. Which term refers to the strategy of optimizing an algorithm's use of resources, often by making sacrifices 
in one aspect for improvements in another?
- [ ] A. Greedy Algorithm
- [ ] B. Divide and Conquer
- [ ] C. Dynamic programming
- [x] D. Trade off

<details>
  <summary> Solution </summary>

```
Greedy Algorithm, Divide and Conquer, Dynamic programming
- These 3 are design technique approaches

```


</details>
<!----------------------------->

---

Q 17. The recurence equation `T(n) = 2T(n-1) + n` represents the time complexity of which algorithm paradigm?
- [ ] A. Dynamic Programming
- [ ] B. Greedy Algorithms
- [x] C. Backtracking
- [ ] D. Iteration

<details>
  <summary> Solution </summary>

```
2T -> 2^n
    which np complete problem
    So, this is solved by backtracking

Iteration = T(n-1) + 1
```


</details>
<!----------------------------->

---

Q 18. What is the time complexity of merge sort for sorting an array of size n?
- [ ] A. O(n)
- [ ] B. O(logn)
- [x] C. O(n logn)
- [ ] D. O(n^2)

<details>
  <summary> Solution </summary>

[Sorting Algo](https://interviewkickstart.com/blogs/learn/time-complexities-of-all-sorting-algorithms)

</details>
<!----------------------------->

---

Q 19. The concept of NP-Completeness was introduced by:
- [x] A. Stephen Cook
- [ ] B. Richard Karn
- [ ] C. Donald Knuth
- [ ] D. John Nash

<details>
  <summary> Solution </summary>

</details>
<!----------------------------->

---

Q 20. What is the main trade-off in **time-space** tradeoff?
- [ ] A. Reducing both time complexity and space complexity simulatenously
- [ ] B. Increasing both time complexity and space complexity simulatenously
- [x] C. Improving time complexity at the cost of space complexity 
- [ ] D. Improving space complexity at the cost increased time complexity

What is the main trade-off in **space-time** tradeoff?
- [ ] A. Reducing both time complexity and space complexity simulatenously
- [ ] B. Increasing both time complexity and space complexity simulatenously
- [ ] C. Improving time complexity at the cost of space complexity 
- [x] D. Improving space complexity at the cost increased time complexity

<details>
  <summary> Solution </summary>

</details>
<!----------------------------->

---

Q 21. Which property of Big-O notation states that if f(n) is O(g(n)), then k*f(n) is O(g(n)) for any positive constant k?
- [ ] A. Transitivity
- [ ] B. Addition
- [x] C. Multiplication
- [ ] D. Reflexivity

<details>
  <summary> Solution </summary>

```
f(n)    ->  O(g(n))= O(n^2)
k*f(n)  ->  O(n^2)
```

</details>
<!----------------------------->

---

Q 22. The recurrence equation `T(n) = T(n/2) + 1` represents the time complexity of which algorithmic paradigm?
- [x] A. Divide and Conquer
- [ ] B. Greedy Algorithms
- [ ] C. Dynamic Programming
- [ ] D. Brute Force

<details>
  <summary> Solution </summary>

```
T(n) = T(n/2) + 1
        n/2 + 1 = log n
So, any algorithm who complexity is log n which of Binary Search
There recurrence relation will be T(n) = T(n/2) + 1
---------------------------------
T(n) = T(n/2) + n
        n log n        -> Merge Sort 
```

</details>
<!----------------------------->

---

Q 23. Merge Sort is an example of a sorting algorithms that uses the Divide and conquer paradigm. What is the time
complexity in the worst case scenario?
- [ ] A. O(n)
- [x] B. O(n log n)
- [ ] C. O(n^2)
- [ ] D. O(log n)

<details>
  <summary> Solution </summary>

</details>
<!----------------------------->

---

Q 24. If a problen A is Np-Complete and another problem B can be reduced to problem A in polynomial time, what can
said about problem B?
- [x] A. Problem B is also NP-Complete
- [ ] B. Problem B is in P
- [ ] C. Problem B is not solvable
- [ ] D. Problem B is not a decision problem

<details>
  <summary> Solution </summary>

</details>
<!----------------------------->

---

Q 25. How many edges are required for a graph with n vertices to be triconnected 
(have atleast 3 biconnected components)?
- [ ] A. n
- [ ] B. n-1
- [ ] C. n-2
- [x] D. It is not possible to determine based on the number of vertices

<details>
  <summary> Solution </summary>

</details>
<!----------------------------->

---

Q 26. In multi-stage graphs, what is the property of optimality?
- [ ] A. The shortest path between any two stages is the one with the fewest edges
- [x] B. The shortest path between any two stages is the one with the lowest total cost
- [ ] C. The shortest path between any two stages is the one with the highest total cost
- [ ] D. The shortest path between any two stages is the one with the most vertices

<details>
  <summary> Solution </summary>

</details>
<!----------------------------->

---

Q 27. Threaded Binary trees are particularly useful for which type of traversal?
- [ ] A. Preorder
- [x] B. Inorder
- [ ] C. Postorder
- [ ] D. Level order

<details>
  <summary> Solution </summary>

</details>
<!----------------------------->

---

Q 28. A complete binary tree is a binary tree in which:
- [ ] A. All nodes have the same value
- [ ] B. All leaf nodes are at the same level
- [ ] C. All internal nodes have the same degree
- [ ] D. The left subtree of each node has a larger height than the right subtree
- [x] E. None

<details>
  <summary> Solution </summary>

[omplete binary tree](https://www.programiz.com/dsa/complete-binary-tree)

</details>
<!----------------------------->

---

Q 29. Which collision resolution technique involves placing collided elements in the next available 
empty slot in the hash table?
- [x] A. Linear probing
- [ ] B. Quadratic probing
- [ ] C. Separate chaining
- [ ] D. Double Hashing

<details>
  <summary> Solution </summary>

[collision resolution technique](https://cexpertvision.com/collision-resolution-techniques/)

</details>
<!----------------------------->

---

Q 30. Index sequential search is an improvement over sequential search that uses:
- [ ] A. Linked lists for effiecient searching
- [x] B. Array for effiecient searching
- [ ] C. Hashing for effiecient searching
- [ ] D. Binary search trees for efficient searching

<details>
  <summary> Solution </summary>

</details>
<!----------------------------->

---

Q 31. In the Tower of Hanoi problem with n disks, how many moves are required to solve the problem?
- [ ] A. n
- [ ] B. 2n
- [x] C. 2^n-1
- [ ] D. 2^n

<details>
  <summary> Solution </summary>

n = 3
2^n-1 =  2^3-1 = 7 

</details>
<!----------------------------->

---

Q 32. Which of the following is not a common example of an abstract data type?
- [ ] A. stack
- [x] B. integer
- [ ] C. queue
- [ ] D. list

<details>
  <summary> Solution </summary>

</details>
<!----------------------------->

---

Q 33. Which type of linked lust is most suitable for implementing a queue data structure?
- [x] A. Singly linked list
- [ ] B. Doubly linked list
- [ ] C. Circular linked list
- [ ] D. Array implementation of linked list

<details>
  <summary> Solution </summary>

[Linked List](https://www.w3schools.com/dsa/dsa_theory_linkedlists.php)

<img width="1017" height="332" alt="image" src="https://github.com/user-attachments/assets/ed3d8f0e-bdae-47f6-ab8b-97b60551ce2b" />


</details>
<!----------------------------->

---

Q 34. A problem is said to be in NP if:
- [x] A. Its solution can be verified in polynomial time
- [ ] B. It can be solved using a non-deterministic algorithm
- [ ] C. It is not solvable
- [ ] D. It has exponential complexity

<details>
  <summary> Solution </summary>

</details>
<!----------------------------->

---

Q 35. The minimum number of edges in a spanning tree of a connected graph with n vertices is:
- [ ] A. n
- [x] B. n-1
- [ ] C. n+1
- [ ] D. n(n-1)2

<details>
  <summary> Solution </summary>

[Minimum Spanning Tree MST](https://www.w3schools.com/dsa/dsa_theory_mst_minspantree.php)

</details>
<!----------------------------->

---

Q 36. In the context of All-Pair Shortest Paths algrithm, what does the term "transitive property" refers to?
- [ ] A. The property of having a cyclic path
- [ ] B. The property of having all vertices connected to each other
- [x] C. The property of being able to reach one vertex from another
- [ ] D. The property of a path being shorter than another path

<details>
  <summary> Solution </summary>

```
Transitive:
A -> B -> C
A -> C
```

</details>
<!----------------------------->

---

Q 37. In a Binary Search Tree(BST), the operation of deleting a node with one child involves:
- [ ] A. Removing the node and replacing it with its left child
- [ ] B. Removing the node and replacing it with its right child
- [x] C. Removing the node and replacing it with its parent
- [ ] D. Removing the node and leaving the subtree unaltered

<details>
  <summary> Solution </summary>

[BST](https://www.w3schools.com/dsa/dsa_data_binarysearchtrees.php)

</details>
<!----------------------------->

---

Q 38. Connected Components in a graph can be found using which graph traversal algorithm?
- [ ] A. DFS
- [ ] B. BFS
- [x] C. Both DFS and BFS
- [ ] D. Nither DFS nor BFS

<details>
  <summary> Solution </summary>

</details>
<!----------------------------->

---

Q 39. Counting Sort is particularly effiecient for sorting arrays where the range of elements is:
- [ ] A. very large
- [x] B. very small
- [ ] C. constant
- [ ] D. sorted

<details>
  <summary> Solution </summary>

[Counting Sort](https://www.w3schools.com/dsa/dsa_algo_countingsort.php)

| Comparision Sorting     | insertion, bubble, selection, merge, heap |
|-------------------------|----------------------------------------|
| Non-Comparision Sorting | Counting sort, Redix sort, Bucket sort | 

</details>
<!----------------------------->

---

Q 40. Which type of queue allows insertion and deletion of elements at both the front and rear ends?
- [ ] A. Circular queue
- [ ] B. Linear queue
- [x] C. Dequeue (Doubly-ended queue)
- [ ] D. Priority queue

<details>
  <summary> Solution </summary>

[Types of Queue](https://www.programiz.com/dsa/types-of-queue)

</details>
<!----------------------------->

---

Q 41. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> Solution </summary>

</details>
<!----------------------------->

---

Q 42. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> Solution </summary>

</details>
<!----------------------------->

---

Q 43. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> Solution </summary>

</details>
<!----------------------------->

---

Q 44. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> Solution </summary>

</details>
<!----------------------------->

---

Q 45. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> Solution </summary>

</details>
<!----------------------------->

---

Q 46. 
- [ ] A.
- [ ] B.
- [ ] C.
- [ ] D.

<details>
  <summary> Solution </summary>

</details>
<!----------------------------->

---
