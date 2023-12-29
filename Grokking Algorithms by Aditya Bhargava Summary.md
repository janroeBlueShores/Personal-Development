# Chapter I
## Introduction to Algorithms

- An algorithm is a set of instructions for accomplishing a task
  - Every piece of code could be called an algorithm
- Binary search is an algorithm where the input is a sorted list of elements
  - is a lot faster than simple search
  - only works when your list is in sorted order (e.g. names in a phone book are sorted in alphabetical order)
- Big O notation is special notation that tells you how fast an algorithm is
- Binary search has run time of O(log n)
  - O(log n) is faster than O(n)
  - Log time or O(log n) gets a lot faster once the list of items you’re searching through grows
- Algorithm speed isn’t measured in seconds
- Algorithm times are measured in terms of growth of an algorithm
- Algorithm times are written in Big O notation

---

# Chapter II
## Selection Sort

- Your computer’s memory is like a giant set of drawers
- When you want to store multiple elements, use an array or a list
- Arrays allow fast reads.
- Linked lists allow fast inserts and deletes.
- With an array, all your elements are stored right next to each other
  - The elements in an array are numbered and starts from 0
  - Almost every programming language you use will number array elements starting at 0
- With a list, elements are strewn all over, and one element stores the address of the next one.
- All elements in the array should be the same type (all ints, all doubles, and so on).
- Selection sort is a neat algorithm, but it’s not very fast (On<sup>2</sup>). Quicksort is a faster sorting algorithm that only takes O(n log n) time.

---

# Chapter III
## Recursion

- Recursion is when a function calls itself
  - When writing a recursive function, you have to tell it when to stop recursing
- Every recursive function has two parts: the base case, and the recursive case
  - The recursive case is when the function calls itself
  - The base case is when the function doesn’t call itself again doesn’t go into an infinite loop.
- A stack has two operations: push and pop.
- All function calls go onto the call stack.
- The call stack can get very large, which takes up a lot of memory.

---

# Chapter IV
## Quicksort

- Divide and Conquer (D&C)
- D&C algorithms are recursive algorithms
- To solve a problem using D&C, there are two steps:
  1. Figure out the base case. This should be the simplest possible case.
  2. Divide or decrease your problem until it becomes the base case.
- D&C works by breaking a problem down into smaller and smaller pieces.
- If you’re using D&C on a list, the base case is probably an empty array or an array with one element.
- Quicksort is a sorting algorithm
  - much faster than selection sort and is frequently used in real life
  - one of the fastest sorting algorithms
  - does not check to see whether the input array is already sorted
  - when implementing quicksort, choose a random element as the pivot
  - average runtime is O(n log n)
- The constant in Big O notation can matter sometimes. That’s why quicksort is faster than merge sort.
- The constant almost never matters for simple search versus binary search, because O(log n) is so much faster than O(n) when your list gets big.

---

# Chapter V
## Hash Tables
- A hash function is a function where you put in a string1 and you get back a number.
  - The hash function knows how big your array is and only returns valid indexes
  - A hash table is a combination of an array and a hash function
- Hash tables are already implemented in most common programming languages.
- For built-in hash tables, assume average case performance: constant time.
- Hash tables are a powerful data structure because they’re so fast and they let you model data in a different way.
- Collisions are bad. You need a hash function that minimizes collisions.
  - A good hash function will give you very few collisions
- Hash tables have really fast search, insert, and delete.
- Hash tables are good for modeling relationships from one item to another item.
- Once your load factor is greater than .07, it’s time to resize your hash table.
- Hash tables are used for caching data (for example, with a web server).
- Hash tables are great for catching duplicates.

---

# Chapter VI
## Breadth-First Search

- A graph models a set of connections.
  - made up of nodes and edge
  - A directed graph has arrows, and the relationship follows the direction of the arrow (rama -> adit means “rama owes adit money”).
  - Undirected graphs don’t have arrows, and the relationship goes both ways (ross - rachel means “ross dated rachel and rachel dated ross”).
- Breadth-first search tells you if there’s a path from A to B.
- If there’s a path, breadth-first search will find the shortest path.
- If you have a problem like “find the shortest X,” try modeling your problem as a graph, and use breadth-first search to solve.
- Queues are FIFO (First In, First Out).
- Stacks are LIFO (Last In, First Out).
- You need to check people in the order they were added to the search list, so the search list needs to be a queue. Otherwise, you won’t get the shortest path.
- Once you check someone, make sure you don’t check them again. Otherwise, you might end up in an infinite loop.

---

# Chapter VII
## Dijkstra's Algorithm

- When working with Dijkstra’s algorithm, each edge in the graph has a number associated with it. These are called weights.
  - A graph with weights is called a weighted graph
  - A graph without weights is called an unweighted graph
- Breadth-first search is used to calculate the shortest path for an unweighted graph.
- Dijkstra’s algorithm is used to calculate the shortest path for a weighted graph.
- Dijkstra’s algorithm works when all the weights are positive.
- If you have negative weights, use the Bellman-Ford algorithm.

---

# Chapter VIII
## Greedy Algorithms

- Greedy algorithms optimize locally, hoping to end up with a global optimum.
- NP-complete problems have no known fast solution.
- If you have an NP-complete problem, your best bet is to use an approximation algorithm.
- Greedy algorithms are easy to write and fast to run, so they make good approximation algorithms.

---

# Chapter IX
## Dynamic Programming

- Dynamic programming starts by solving subproblems and builds up to solving the big problem.
  - useful when you’re trying to optimize something given a constraint.
  - can be used when the problem can be broken into discrete subproblems.
- Every dynamic-programming solution involves a grid.
- The values in the cells are usually what you’re trying to optimize.
- Each cell is a subproblem, so think about how you can divide your problem into subproblems.
- There’s no single formula for calculating a dynamic-programming solution.
  
---

# Chapter X
## K-nearest

- KNN is used for classification and regression and involves looking at the k-nearest neighbors.
- Classification = categorization into a group.
- Regression = predicting a response (like a number).
- Feature extraction means converting an item (like a fruit or a user) into a list of numbers that can be compared.
- Picking good features is an important part of a successful KNN algorithm.

