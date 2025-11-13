# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. What are some things that you learned through this assignment? Think about the concepts of backtracking, constraint satisfaction, and search algorithms. Were there any particular challenges you faced while implementing the Board class methods or the DFS/BFS functions? How did you overcome them?
I learned how a depth first and breadth first search algorithm works. In AP CSA, I learned how recursive functions work and I understood them, but I had never seen like an actual application of using them. To do DFS, i had to use recursion and it was interesting to see how it works and backtracks. The challenge I faced while implementing the methods was the BFS methods, I didnt really understand how it would work within the sudoku problem. I overcame them by asking chatgpt and my friends how you would do the method. To me, DFS made much more sense naturally because its similar to how some poeple play sudoku. 


2. How can you apply what you learned in this assignment to future programs or projects? Consider other types of problems that involve searching through possibilities, making decisions, and backtracking when those decisions don't work out. Can you think of real-world scenarios where DFS or BFS might be useful? What about other constraint satisfaction problems?
Now that I have learned how to use DFS and BFS I can know when to implement a method that can backtrack. These can be used in many other algorithms in other games or puzzles. Some real world scenarios where these types of algorithms could be useful (especially BFS) is finding the shortest path within something. For example, finding the shortest series of moves to solve a rubiks cube. For DFS you could solve to find a path, but it might not be the most efficient one. 


3. Explain how the Stack and Queue classes work and why they are important for DFS and BFS algorithms. Describe the difference between LIFO (Last In First Out) and FIFO (First In First Out) data structures. How does using a Stack versus a Queue change the way the search algorithm explores possible solutions? Why is one data structure better suited for depth-first search and the other for breadth-first search?
Stack is a type of data structure that is LIFO, like a stack of books. A queue is a data structure that is like a line, that follows the FIFO rule. The difference in BFS and DFS is the order they explore/find each state. In DFS you go deep into one path and you backtrack when you fail, a stack works well here because you can push each time you go deeper, and when you fail, you pop to backtrack.  In BFS you go level by level and you dont backtrack, a queue is good for this because the earliest states get expanded first and it explores everything level by level before going deeper. 