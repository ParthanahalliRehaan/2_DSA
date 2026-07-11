# 🎯 The 150-Qn DSA Mastery Plan: 50 Dawns

**Format per Dawn:** 1 Conceptual Read + 3 Pattern-Based Questions (Blind Solve)

---

## Phase 1: Foundations — Arrays, Strings, Hashing, Two Pointers, Sliding Window (Dawns 1-10)

| Dawn | Conceptual Read | Pattern Block (3 Qns — Blind Solve) |
|:---|:---|:---|
| **Dawn 1** | **Time Complexity & Space Complexity** — Orders of growth, how to derive TC from loops, nested loops, recursion tree. Best/Worst/Average case intuition. | 1. [Two Sum](https://leetcode.com/problems/two-sum/) → Hashing O(n)<br>2. [Contains Duplicate](https://leetcode.com/problems/contains-duplicate/) → Hash set pattern<br>3. [Valid Anagram](https://leetcode.com/problems/valid-anagram/) → Frequency array/hash |
| **Dawn 2** | **Asymptotic Notations** — Big-O, Big-Theta, Big-Omega formal definitions. Proving f(n) = O(g(n)). Common pitfalls (drop constants, lower order terms). | 1. [Best Time to Buy/Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/) → One pass O(n)<br>2. [Maximum Subarray (Kadane's)](https://leetcode.com/problems/maximum-subarray/) → Greedy local max<br>3. [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self/) → Prefix/suffix product |
| **Dawn 3** | **Two Pointers Technique** — When to use (sorted arrays, palindromes, pair sums). Fast-slow pattern. Shrinking window pattern. | 1. [Two Sum II (sorted)](https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/) → Classic two pointers<br>2. [3Sum](https://leetcode.com/problems/3sum/) → Sort + two pointers + skip duplicates<br>3. [Container With Most Water](https://leetcode.com/problems/container-with-most-water/) → Shrinking from ends |
| **Dawn 4** | **Sliding Window (Fixed Size)** — Window formation, maintaining state, sliding logic. When NOT to use. | 1. [Maximum Average Subarray I](https://leetcode.com/problems/maximum-average-subarray-i/) → Basic fixed window<br>2. [Substring with Concatenation of All Words](https://leetcode.com/problems/substring-with-concatenation-of-all-words/) → Hash + fixed window<br>3. [Sliding Window Maximum](https://leetcode.com/problems/sliding-window-maximum/) → Monotonic deque (bridge to next) |
| **Dawn 5** | **Sliding Window (Variable Size)** — Expanding/shrinking, condition-based window. Longest/shortest subarray patterns. | 1. [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters/) → Hash set + shrink<br>2. [Minimum Size Subarray Sum](https://leetcode.com/problems/minimum-size-subarray-sum/) → Shrink when valid<br>3. [Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring/) → Hard variable window |
| **Dawn 6** | **Prefix Sum & Difference Array** — Building prefix sums, range queries, subarray sum patterns. 2D prefix sum concept. | 1. [Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k/) → Prefix sum + hash map<br>2. [Continuous Subarray Sum](https://leetcode.com/problems/continuous-subarray-sum/) → Prefix sum + modulo<br>3. [Range Sum Query - Immutable](https://leetcode.com/problems/range-sum-query-immutable/) → Classic prefix sum |
| **Dawn 7** | **Strings: Basic Manipulation & Patterns** — String builder efficiency, palindrome checks, anagram groups. | 1. [Group Anagrams](https://leetcode.com/problems/group-anagrams/) → Sort key / frequency key<br>2. [Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring/) → Expand around center<br>3. [Palindromic Substrings](https://leetcode.com/problems/palindromic-substrings/) → Count all centers |
| **Dawn 8** | **Stack: Basic Operations & Applications** — LIFO principle, expression evaluation, bracket matching. | 1. [Valid Parentheses](https://leetcode.com/problems/valid-parentheses/) → Classic stack<br>2. [Min Stack](https://leetcode.com/problems/min-stack/) → Auxiliary stack pattern<br>3. [Evaluate Reverse Polish Notation](https://leetcode.com/problems/evaluate-reverse-polish-notation/) → Stack evaluation |
| **Dawn 9** | **Monotonic Stack** — Increasing/decreasing stack, next greater/smaller element. Why monotonicity helps. | 1. [Next Greater Element I](https://leetcode.com/problems/next-greater-element-i/) → Monotonic decreasing<br>2. [Daily Temperatures](https://leetcode.com/problems/daily-temperatures/) → Waiting days pattern<br>3. [Largest Rectangle in Histogram](https://leetcode.com/problems/largest-rectangle-in-histogram/) → Hard monotonic |
| **Dawn 10** | **Queue, Deque & Circular Queue** — FIFO, circular array implementation, double-ended operations. | 1. [Design Circular Queue](https://leetcode.com/problems/design-circular-queue/) → Implementation<br>2. [Sliding Window Maximum](https://leetcode.com/problems/sliding-window-maximum/) → Monotonic deque (revisit)<br>3. [Design Front Middle Back Queue](https://leetcode.com/problems/design-front-middle-back-queue/) → Deque operations |

---

## Phase 2: Linked Lists & Binary Trees (Dawns 11-20)

| Dawn | Conceptual Read | Pattern Block |
|:---|:---|:---|
| **Dawn 11** | **Singly Linked List: Reversal & Traversal** — Pointer manipulation, iterative vs recursive reversal. Edge cases (empty, single node). | 1. [Reverse Linked List](https://leetcode.com/problems/reverse-linked-list/) → Iterative reversal<br>2. [Reverse Linked List II](https://leetcode.com/problems/reverse-linked-list-ii/) → Reverse sublist<br>3. [Palindrome Linked List](https://leetcode.com/problems/palindrome-linked-list/) → Find middle + reverse + compare |
| **Dawn 12** | **Slow-Fast Pointer (Floyd's Cycle)** — Cycle detection, finding entry point, mathematical proof of why it works. | 1. [Linked List Cycle](https://leetcode.com/problems/linked-list-cycle/) → Basic detection<br>2. [Linked List Cycle II](https://leetcode.com/problems/linked-list-cycle-ii/) → Find entry node<br>3. [Find the Duplicate Number](https://leetcode.com/problems/find-the-duplicate-number/) → Floyd's on array |
| **Dawn 13** | **Merge Patterns on Linked Lists** — Merge two sorted, merge K sorted strategies. | 1. [Merge Two Sorted Lists](https://leetcode.com/problems/merge-two-sorted-lists/) → Iterative merge<br>2. [Merge K Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists/) → Min-heap / divide-conquer<br>3. [Sort List](https://leetcode.com/problems/sort-list/) → Merge sort on linked list |
| **Dawn 14** | **Doubly Linked List & LRU Cache Design** — Why doubly linked for O(1) removal, hash map + DLL combo. | 1. [LRU Cache](https://leetcode.com/problems/lru-cache/) → Hash + DLL<br>2. [Design Browser History](https://leetcode.com/problems/design-browser-history/) → DLL navigation<br>3. [All O`one Data Structure](https://leetcode.com/problems/all-oone-data-structure/) → Hard DLL + hash |
| **Dawn 15** | **Binary Tree: Properties & DFS Traversals** — Height, depth, size. Inorder/preorder/postorder recursive & iterative. | 1. [Maximum Depth of Binary Tree](https://leetcode.com/problems/maximum-depth-of-binary-tree/) → Basic DFS<br>2. [Binary Tree Inorder Traversal](https://leetcode.com/problems/binary-tree-inorder-traversal/) → Iterative with stack<br>3. [Binary Tree Preorder Traversal](https://leetcode.com/problems/binary-tree-preorder-traversal/) → Morris traversal |
| **Dawn 16** | **Binary Tree: BFS & Level-Order** — Queue-based level order, level-by-level processing, zigzag pattern. | 1. [Binary Tree Level Order Traversal](https://leetcode.com/problems/binary-tree-level-order-traversal/) → Classic BFS<br>2. [Binary Tree Zigzag Level Order](https://leetcode.com/problems/binary-tree-zigzag-level-order-traversal/) → Flag direction<br>3. [Binary Tree Right Side View](https://leetcode.com/problems/binary-tree-right-side-view/) → Last node per level |
| **Dawn 17** | **Binary Tree: Path & Sum Problems** — Root-to-leaf paths, path sum, max path. Post-order processing. | 1. [Path Sum](https://leetcode.com/problems/path-sum/) → DFS target sum<br>2. [Path Sum II](https://leetcode.com/problems/path-sum-ii/) → Track all paths<br>3. [Binary Tree Maximum Path Sum](https://leetcode.com/problems/binary-tree-maximum-path-sum/) → Hard post-order |
| **Dawn 18** | **Binary Search Tree: Properties & Operations** — BST definition, search, insert, delete. Why O(h) time. | 1. [Validate Binary Search Tree](https://leetcode.com/problems/validate-binary-search-tree/) → Range check / inorder<br>2. [Lowest Common Ancestor of BST](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-search-tree/) → BST property<br>3. [Insert into a Binary Search Tree](https://leetcode.com/problems/insert-into-a-binary-search-tree/) → BST insert |
| **Dawn 19** | **BST: Advanced Operations & Kth Element** — Inorder successor, predecessor, Kth smallest/largest. Morris traversal for O(1) space. | 1. [Kth Smallest Element in a BST](https://leetcode.com/problems/kth-smallest-element-in-a-bst/) → Inorder count<br>2. [Balance a Binary Search Tree](https://leetcode.com/problems/balance-a-binary-search-tree/) → DSW / inorder + build<br>3. [Closest Binary Search Tree Value](https://leetcode.com/problems/closest-binary-search-tree-value/) → BST prune |
| **Dawn 20** | **Balanced Trees: AVL Concepts** — Balance factor, rotations (LL, RR, LR, RL). Why height-balanced matters. Read-only, no code required. | 1. [Convert Sorted Array to BST](https://leetcode.com/problems/convert-sorted-array-to-binary-search-tree/) → Height balanced<br>2. [Balance a Binary Search Tree](https://leetcode.com/problems/balance-a-binary-search-tree/) → Revisit / AVL spirit<br>3. [Design Add and Search Words Data Structure](https://leetcode.com/problems/design-add-and-search-words-data-structure/) → Trie-like tree |

---

## Phase 3: Recursion, Backtracking & Divide-Conquer (Dawns 21-30)

| Dawn | Conceptual Read | Pattern Block |
|:---|:---|:---|
| **Dawn 21** | **Recursion Fundamentals** — Base case, recursive case, call stack visualization. Tail recursion. Common mistakes (missing base case). | 1. [Climbing Stairs](https://leetcode.com/problems/climbing-stairs/) → Fibonacci recursion<br>2. [Fibonacci Number](https://leetcode.com/problems/fibonacci-number/) → Pure recursion + memo<br>3. [Power of Three](https://leetcode.com/problems/power-of-three/) → Recursive check |
| **Dawn 22** | **Recurrence Relations: Solving Methods** — Iteration method, substitution method, recursion tree method. Building intuition for closed forms. | 1. [Pow(x, n)](https://leetcode.com/problems/powx-n/) → Binary exponentiation D&C<br>2. [Different Ways to Add Parentheses](https://leetcode.com/problems/different-ways-to-add-parentheses/) → Catalan-style D&C<br>3. [Unique Binary Search Trees](https://leetcode.com/problems/unique-binary-search-trees/) → Catalan DP |
| **Dawn 23** | **Master Theorem** — All 3 cases, when it applies, when it fails. Practice identifying a, b, f(n). | 1. [Sort an Array](https://leetcode.com/problems/sort-an-array/) → Merge sort implementation<br>2. [Reverse Pairs](https://leetcode.com/problems/reverse-pairs/) → Modified merge sort D&C<br>3. [Count of Smaller Numbers After Self](https://leetcode.com/problems/count-of-smaller-numbers-after-self/) → Fenwick/merge sort |
| **Dawn 24** | **Backtracking: Subset Pattern** — Decision tree, include/exclude, state space. Power set generation. | 1. [Subsets](https://leetcode.com/problems/subsets/) → Classic backtracking<br>2. [Subsets II](https://leetcode.com/problems/subsets-ii/) → Skip duplicates<br>3. [Combination Sum](https://leetcode.com/problems/combination-sum/) → Unbounded choice |
| **Dawn 25** | **Backtracking: Permutation Pattern** — Swap-based vs used-array approach. Handling duplicates. | 1. [Permutations](https://leetcode.com/problems/permutations/) → Swap backtrack<br>2. [Permutations II](https://leetcode.com/problems/permutations-ii/) → Sort + skip duplicates<br>3. [Next Permutation](https://leetcode.com/problems/next-permutation/) → In-place lexicographic |
| **Dawn 26** | **Backtracking: Constraint Satisfaction** — Pruning, forward checking, state validity. N-Queens state representation. | 1. [N-Queens](https://leetcode.com/problems/n-queens/) → Your syllabus!<br>2. [N-Queens II](https://leetcode.com/problems/n-queens-ii/) → Count only<br>3. [Sudoku Solver](https://leetcode.com/problems/sudoku-solver/) → Constraint backtracking |
| **Dawn 27** | **Backtracking: Graph Coloring & Combinatorial** — M-coloring problem, bipartite check as 2-coloring. | 1. [Graph Valid Tree](https://leetcode.com/problems/graph-valid-tree/) → Union-find / DFS<br>2. [Is Graph Bipartite?](https://leetcode.com/problems/is-graph-bipartite/) → 2-coloring BFS/DFS<br>3. [Flower Planting With No Adjacent](https://leetcode.com/problems/flower-planting-with-no-adjacent/) → M-coloring simple |
| **Dawn 28** | **Quick Sort & Partition Schemes** — Lomuto vs Hoare partition. Randomized pivot. Why O(n²) worst case, O(n log n) average. | 1. [Sort Colors](https://leetcode.com/problems/sort-colors/) → Dutch national flag (3-way)<br>2. [Kth Largest Element in Array](https://leetcode.com/problems/kth-largest-element-in-an-array/) → Quickselect<br>3. [Wiggle Sort II](https://leetcode.com/problems/wiggle-sort-ii/) → Median + three-way partition |
| **Dawn 29** | **Merge Sort & Divide-Conquer Analysis** — Stable sort, merge procedure, time/space analysis. Inversion count intuition. | 1. [Count of Range Sum](https://leetcode.com/problems/count-of-range-sum/) → D&C + prefix sum<br>2. [The Skyline Problem](https://leetcode.com/problems/the-skyline-problem/) → D&C sweep line<br>3. [Expression Add Operators](https://leetcode.com/problems/expression-add-operators/) → Backtrack + eval |
| **Dawn 30** | **Karatsuba Multiplication** — Divide numbers, 3 multiplications instead of 4. Strassen's concept (read-only). When D&C beats naive. | 1. [Multiply Strings](https://leetcode.com/problems/multiply-strings/) → Simulate / grade school<br>2. [Add Strings](https://leetcode.com/problems/add-strings/) → Two pointers add<br>3. [Divide Two Integers](https://leetcode.com/problems/divide-two-integers/) → Binary division D&C |

---

## Phase 4: Graphs, Greedy & Dynamic Programming (Dawns 31-42)

| Dawn | Conceptual Read | Pattern Block |
|:---|:---|:---|
| **Dawn 31** | **Graph Representation: Adjacency List vs Matrix** — Space tradeoffs, when to use which. Edge list for Kruskal. | 1. [Find if Path Exists in Graph](https://leetcode.com/problems/find-if-path-exists-in-graph/) → Basic DFS/BFS<br>2. [Find the Town Judge](https://leetcode.com/problems/find-the-town-judge/) → In-degree / out-degree<br>3. [Course Schedule](https://leetcode.com/problems/course-schedule/) → Topological sort |
| **Dawn 32** | **Graph BFS & DFS Traversals** — Connected components, flood fill, grid graphs. Visited set importance. | 1. [Number of Islands](https://leetcode.com/problems/number-of-islands/) → DFS grid<br>2. [Max Area of Island](https://leetcode.com/problems/max-area-of-island/) → DFS area count<br>3. [Pacific Atlantic Water Flow](https://leetcode.com/problems/pacific-atlantic-water-flow/) → Multi-source BFS/DFS |
| **Dawn 33** | **Topological Sort: Kahn's Algorithm & DFS** — In-degree method, detecting cycles in directed graph. | 1. [Course Schedule II](https://leetcode.com/problems/course-schedule-ii/) → Return order<br>2. [Alien Dictionary](https://leetcode.com/problems/alien-dictionary/) → Build graph + topo sort<br>3. [Sequence Reconstruction](https://leetcode.com/problems/sequence-reconstruction/) → Verify unique topo order |
| **Dawn 34** | **Shortest Path: Dijkstra's Algorithm** — Greedy, priority queue, relaxation. Why no negative edges. Time complexity analysis. | 1. [Network Delay Time](https://leetcode.com/problems/network-delay-time/) → Classic Dijkstra<br>2. [Cheapest Flights Within K Stops](https://leetcode.com/problems/cheapest-flights-within-k-stops/) → Modified Dijkstra<br>3. [Path With Maximum Probability](https://leetcode.com/problems/path-with-maximum-probability/) → Max probability Dijkstra |
| **Dawn 35** | **Union-Find (Disjoint Set Union)** — Path compression, union by rank/size. Amortized analysis (inverse Ackermann). | 1. [Number of Provinces](https://leetcode.com/problems/number-of-provinces/) → Union-find<br>2. [Redundant Connection](https://leetcode.com/problems/redundant-connection/) → Detect cycle<br>3. [Accounts Merge](https://leetcode.com/problems/accounts-merge/) → Union-find + hash |
| **Dawn 36** | **Minimum Spanning Tree: Prim's Algorithm** — Greedy, cut property, priority queue implementation. | 1. [Min Cost to Connect All Points](https://leetcode.com/problems/min-cost-to-connect-all-points/) → Prim's / Kruskal's<br>2. [Optimize Water Distribution in a Village](https://leetcode.com/problems/optimize-water-distribution-in-a-village/) → Prim's with virtual node<br>3. [Find Critical and Pseudo-Critical Edges in MST](https://leetcode.com/problems/find-critical-and-pseudo-critical-edges-in-mst/) → Hard MST |
| **Dawn 37** | **Minimum Spanning Tree: Kruskal's Algorithm** — Sort edges, union-find, cycle detection. Cut property proof intuition. | 1. [Min Cost to Connect All Points](https://leetcode.com/problems/min-cost-to-connect-all-points/) → Kruskal's revisit<br>2. [Connecting Cities With Minimum Cost](https://leetcode.com/problems/connecting-cities-with-minimum-cost/) → Kruskal's<br>3. [Find the City With the Smallest Number of Neighbors at a Threshold Distance](https://leetcode.com/problems/find-the-city-with-the-smallest-number-of-neighbors-at-a-threshold-distance/) → Floyd-Warshall |
| **Dawn 38** | **Greedy Algorithm Design & Proof** — Greedy choice property, optimal substructure. Activity selection, interval scheduling. Huffman coding concept. | 1. [Non-overlapping Intervals](https://leetcode.com/problems/non-overlapping-intervals/) → Greedy proof<br>2. [Merge Intervals](https://leetcode.com/problems/merge-intervals/) → Sort + greedy<br>3. [Meeting Rooms II](https://leetcode.com/problems/meeting-rooms-ii/) → Min-heap greedy |
| **Dawn 39** | **Greedy: Huffman Coding & Advanced** — Prefix-free codes, optimal merge pattern. When greedy fails (0/1 knapsack vs fractional). | 1. [Minimum Cost to Connect Sticks](https://leetcode.com/problems/minimum-cost-to-connect-sticks/) → Huffman-like greedy<br>2. [Task Scheduler](https://leetcode.com/problems/task-scheduler/) → Greedy + math<br>3. [Reorganize String](https://leetcode.com/problems/reorganize-string/) → Greedy + max-heap |
| **Dawn 40** | **Dynamic Programming: Introduction & 1D DP** — Memoization vs tabulation. Overlapping subproblems, optimal substructure. Bottom-up intuition. | 1. [Climbing Stairs](https://leetcode.com/problems/climbing-stairs/) → DP revisit<br>2. [House Robber](https://leetcode.com/problems/house-robber/) → Decision DP<br>3. [House Robber II](https://leetcode.com/problems/house-robber-ii/) → Circular DP |
| **Dawn 41** | **DP: 2D Grid & Path Problems** — Grid traversal, unique paths, obstacle handling. Space optimization. | 1. [Unique Paths](https://leetcode.com/problems/unique-paths/) → Grid DP<br>2. [Unique Paths II](https://leetcode.com/problems/unique-paths-ii/) → Obstacles<br>3. [Minimum Path Sum](https://leetcode.com/problems/minimum-path-sum/) → Min path grid |
| **Dawn 42** | **DP: Longest Common Subsequence (LCS)** — Your syllabus! LCS recurrence, print LCS, space optimization to O(min(m,n)). | 1. [Longest Common Subsequence](https://leetcode.com/problems/longest-common-subsequence/) → Classic LCS<br>2. [Longest Palindromic Subsequence](https://leetcode.com/problems/longest-palindromic-subsequence/) → LCS with reverse<br>3. [Edit Distance](https://leetcode.com/problems/edit-distance/) → LCS variant |

---

## Phase 5: Advanced DP, Graph DP & Hard Patterns (Dawns 43-50)

| Dawn | Conceptual Read | Pattern Block |
|:---|:---|:---|
| **Dawn 43** | **DP: Knapsack Variants** — 0/1 knapsack, unbounded knapsack, space optimization. Subset sum, partition equal subset. | 1. [Partition Equal Subset Sum](https://leetcode.com/problems/partition-equal-subset-sum/) → 0/1 knapsack<br>2. [Coin Change](https://leetcode.com/problems/coin-change/) → Unbounded knapsack<br>3. [Coin Change II](https://leetcode.com/problems/coin-change-ii/) → Count combinations |
| **Dawn 44** | **DP: Matrix Chain Multiplication Concept** — Your syllabus! Parenthesization, optimal split point, O(n³) solution. | 1. [Burst Balloons](https://leetcode.com/problems/burst-balloons/) → Interval DP (MCM spirit)<br>2. [Minimum Cost Tree From Leaf Values](https://leetcode.com/problems/minimum-cost-tree-from-leaf-values/) → MCM-like<br>3. [Strange Printer](https://leetcode.com/problems/strange-printer/) → Interval DP |
| **Dawn 45** | **DP on Trees** — Post-order DP, tree diameter, max path sum revisit. Rerooting technique concept. | 1. [House Robber III](https://leetcode.com/problems/house-robber-iii/) → Tree DP<br>2. [Binary Tree Cameras](https://leetcode.com/problems/binary-tree-cameras/) → State DP on tree<br>3. [Longest Path With Different Adjacent Characters](https://leetcode.com/problems/longest-path-with-different-adjacent-characters/) → Tree DP |
| **Dawn 46** | **DP on Strings: Advanced** — Wildcard matching, regex matching, interleaving strings. State machine thinking. | 1. [Wildcard Matching](https://leetcode.com/problems/wildcard-matching/) → Two-pointer + DP<br>2. [Regular Expression Matching](https://leetcode.com/problems/regular-expression-matching/) → Hard string DP<br>3. [Interleaving String](https://leetcode.com/problems/interleaving-string/) → 2D string DP |
| **Dawn 47** | **Trie (Prefix Tree)** — Node structure, insert/search/startsWith. Space-time tradeoff. | 1. [Implement Trie](https://leetcode.com/problems/implement-trie-prefix-tree/) → Build from scratch<br>2. [Word Search II](https://leetcode.com/problems/word-search-ii/) → Trie + backtrack<br>3. [Replace Words](https://leetcode.com/problems/replace-words/) → Trie prefix replace |
| **Dawn 48** | **Bit Manipulation & DP with Bits** — XOR properties, counting bits, bitmask DP concept. | 1. [Single Number](https://leetcode.com/problems/single-number/) → XOR<br>2. [Counting Bits](https://leetcode.com/problems/counting-bits/) → DP + bits<br>3. [Maximum XOR of Two Numbers in an Array](https://leetcode.com/problems/maximum-xor-of-two-numbers-in-an-array/) → Trie + bits |
| **Dawn 49** | **Segment Tree / Fenwick Tree (BIT) Concepts** — Range queries, point updates. Lazy propagation concept. When to use. | 1. [Range Sum Query - Mutable](https://leetcode.com/problems/range-sum-query-mutable/) → Segment tree<br>2. [Count of Smaller Numbers After Self](https://leetcode.com/problems/count-of-smaller-numbers-after-self/) → Fenwick tree<br>3. [The Number of Weak Characters in the Game](https://leetcode.com/problems/the-number-of-weak-characters-in-the-game/) → Sort + Fenwick |
| **Dawn 50** | **Proof of Correctness & Complexity Analysis Mastery** — Loop invariants, induction, contradiction. Final synthesis of all asymptotic analysis. | 1. [First Missing Positive](https://leetcode.com/problems/first-missing-positive/) → O(n) time O(1) space proof<br>2. [Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays/) → Binary search proof<br>3. [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water/) → Two pointers correctness proof |

---

## 📊 Coverage Checklist vs Your Syllabus

| Module | Coverage |
|:---|:---|
| **Module 1: Algorithm Analysis** | ✅ Fully covered (Dawns 1-3, 22-23, 28-29, 50) |
| **Module 2: Linear DS** | ✅ Fully covered (Dawns 1-14) |
| **Module 2: Binary Trees** | ✅ Fully covered (Dawns 15-20) |
| **Module 2: Graphs** | ✅ Fully covered (Dawns 31-37) |
| **Module 2: Hashing** | ✅ Covered throughout (hash maps in many dawns) |
| **Module 3: Divide & Conquer** | ✅ Fully covered (Dawns 22-23, 28-30) |
| **Module 3: Backtracking** | ✅ Fully covered (Dawns 24-27) |
| **Module 3: Branch & Bound** | ⚠️ Conceptually covered via backtracking + pruning (Dawns 26-27). LIFO/FIFO-BB, Job Selection, Subset Sum are theoretical — read Cormen but skip coding. |
| **Module 4: Greedy** | ✅ Fully covered (Dawns 34, 36-39) |
| **Module 4: Dynamic Programming** | ✅ Fully covered (Dawns 40-46) |
| **Module 5: Complexity Classes** | ❌ Discarded as requested |
| **Module 5: Approximation Algorithms** | ❌ Discarded as requested |

---

## 🗂️ Your Doc Template (Per Dawn)

```markdown
# Dawn XX: [Concept Name]

## Conceptual Read
- Source: Cormen Ch X / TakeUForward / Self-derived
- Key points:
- Time/Space complexity rules:
- Proof / Intuition:

## Pattern: [Pattern Name]
- When to use:
- Template (pseudocode):
- Common pitfalls:

## Blind Solve Log
| # | Problem | First Attempt | Final  | Time | Notes |
|---|---------|---------------|--------|------|-------|
| 1 |         | ✅/❌        | ✅/❌ |      |       |
| 2 |         | ✅/❌        | ✅/❌ |      |       |
| 3 |         | ✅/❌        | ✅/❌ |      |       |

## Proof of Correctness (for hardest problem)
- Loop invariant / Base case / Inductive step:
```

---

## 🏁 Rules

1. **Concept first, always.** 20-30 mins reading before touching LeetCode.
2. **Blind solve.** Stuck >20 mins → peek at approach hint only, reset, retry.
3. **One language.** C++ recommended (matches your textbook references).
4. **Document everything.** Your docs are your revision material.
5. **No skipping.** Even "easy" dawns build pattern muscle.

**50 Dawns × 3 Qns = 150 questions. ~25 weeks. Start this weekend.** 🔥