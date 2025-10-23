# Data Structure and Algorithms.

## Core concepts:

Arrays

Strings

Linked List

Stacks and Queues

Recursion

Sorting & Searching

HashMap / HashSet

Trees (Binary Tree, BST)

Heaps & PriorityQueue

Graphs

Dynamic Programming

## DSA problem solvig Patterns

### A. Array & String Patterns

#### Two Pointers

Move two pointers from start/end to solve problems like sum, palindrome, subarrays.

Example: Find two numbers in a sorted array that sum to target.

#### Sliding Window

Maintain a "window" of elements to solve subarray/subsequence problems.

Example: Maximum sum subarray of size k, longest substring with distinct characters.

#### Prefix Sum

Precompute cumulative sums to answer range sum queries efficiently.

Example: Subarray sum equals k problem.

#### Kadane’s Algorithm

Maximum subarray sum problem.

#### Cyclic / Rotation Patterns

Circular arrays, rotate problems, mod operations.

#### Frequency Counting / Hashing

Count occurrences or find duplicates.

Example: Two sum, anagrams, majority element.

### B. Sorting & Searching Patterns

#### Binary Search

Find an element or boundary in sorted arrays.

Variants: lower_bound, upper_bound, rotated array search.

#### Sorting & Two-Pointer / Greedy

Problems where sorting simplifies the solution.

Example: Meeting rooms problem, maximum pairs.

### C. Linked List Patterns

#### Fast & Slow Pointers

Detect cycle, middle of list.

#### Reversing Linked List

Reverse iteratively/recursively.

#### Merge / Split Patterns

Merge two sorted lists, split at middle, etc.

### D. Recursion & Backtracking

#### Subsets / Permutations / Combinations

Maze / Grid / Path Problems

DFS / BFS for Trees & Graphs

### F. Dynamic Programming Patterns

#### 1D DP

Fibonacci, climbing stairs, max sum subsequence.

#### 2D DP

Grid paths, matrix chain multiplication, LCS.

#### DP on Subsequences

LIS, LCS, palindrome subsequences.

### Tricks to handle constraints.

#### step 1 : Check input size --> decide time complexity

Input size(n) --> Allowed complexity -> Trick

n <= 10^2 ---> O(n^2) fine -----> brute force works.
n <= 10^3 ---> O(n^2) may be -----> try for O(nlogn) if possible
n <= 10^5 ---> O(n) or O(nlogn) -----> brute force works.
n<= 10^7 + ---> O(n) or O(n) -----> Avoid loops.

#### step 2: Check value range --> Choose Data structure.

Value Range ---- > Trick
Small (<= 10^4, >=0) --> Can use frequency arrays.
Large (<= 10^9,-19^9 <= val <= 10^9) --> Use HashMap / Set , to avoid frequency array.

Negative numbers present ---> Sliding windows for sum may not work with negatives.

Very large sum ----> Use long in java or check overflow.

#### step 3: check for special cases. (Edge case list):

Always ask:

Can the array be empty?

Can the array have 1 element?

Can all elements be the same?

Can numbers be negative or zero?

Can no solution exist?

Trick: Memorize “0,1,n-1, max, min” → always test these boundaries.

#### step 4: Check Input type/properties.

property -------------> Pattern

1.Sorted array -------------> Two pointers/ Binary search
2.Unsorted array,samll n ------> Brute force possible.
3.Positive numbers only --------> Sliding windows for sum works.
4.String,palindrome chack -------> Two pointers
5.Grid/matrix ------------------->DFS/BFS.
6.Graph ------------------------> BFS/DFS/Dijikstra.
