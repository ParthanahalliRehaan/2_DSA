# 🌳 DSA Master Plan (C++ Track)
> https://www.youtube.com/watch?v=DMeD8trbj6A&t=214s & https://leetcode.com/quest/data-structures-and-algorithms-quest/
> OR
> Basic → Advanced | Tree mapped to daily schedule | 100 days
> Rule: Never skip revision days. Stuck 25 min → see solution → re-solve next day.

---

## THE TREE → DAY MAPPING

```
🌳 DSA (C++)
│
├── 0. FOUNDATIONS ────────────────────────── Days 1–3
│   ├── TC: Big O/Ω/Θ, O(1) → O(n!), amortized, best/avg/worst
│   ├── SC: auxiliary vs total, in-place, recursion stack
│   ├── Recursion: base/recursive case, recursion tree, tail recursion
│   └── Problem-solving: pseudocode → dry run → brute force → optimize
│
├── 1. ARRAYS ─────────────────────────────── Days 4–14
│   ├── Basics: contiguous memory, insert/delete O(n), search, rotate
│   ├── Two Pointers (opposite ends / same direction)
│   ├── Sliding Window (fixed / variable)
│   ├── Prefix Sum, Kadane's
│   ├── Sorting: bubble/selection/insertion → merge/quick/heap
│   ├── Binary Search on Answer
│   └── Patterns: Dutch flag, next permutation, intervals, stock
│
├── 2. STRINGS + HASHING ──────────────────── Days 15–19
│   ├── Palindrome, anagram, KMP/Rabin-Karp
│   └── HashMap/HashSet internals, collisions, rolling hash
│
├── 3. LINKED LIST ────────────────────────── Days 20–26
│   ├── Singly/Doubly/Circular, O(1) insert
│   ├── Fast & Slow pointers, reversal, middle node
│   └── Merge lists, Remove Nth, LRU Cache
│
├── 4. STACK ──────────────────────────────── Days 27–32
│   ├── LIFO, array/LL implementation
│   ├── NGE/NSE ⭐, stock span, largest rectangle ⭐, min stack
│   └── Monotonic stack
│
├── 5. QUEUE ──────────────────────────────── Days 31 (with stack impls)
│   ├── FIFO, circular queue, deque, priority queue → heap
│   └── BFS, sliding window max
│
├── 6. BINARY SEARCH DEEP DIVE ────────────── Days 33–36
│   └── Classic BS, peak element, BS on answer, rotated array
│
├── 7. TREES ──────────────────────────────── Days 37–47
│   ├── BT: traversals (in/pre/post/level), height, diameter, LCA,
│   │   views, serialize ⭐, max path sum ⭐
│   ├── BST: search/insert/delete, validate, kth smallest, floor/ceil
│   └── Advanced: AVL, Red-Black, Segment/Fenwick tree
│
├── 8. HEAP / PRIORITY QUEUE ──────────────── Days 48–51
│   └── Min/max heap, heapify O(n), kth largest, median of stream ⭐
│
├── 9. GRAPHS ⭐ ──────────────────────────── Days 58–69
│   ├── Adj matrix/list, BFS, DFS
│   ├── Dijkstra, Bellman-Ford, Floyd-Warshall
│   ├── Topological sort (Kahn's), MST (Prim's/Kruskal's)
│   ├── Union-Find ⭐ (path compression, union by rank)
│   └── Bridges, SCC, bipartite
│
├── 10. BACKTRACKING ──────────────────────── Days 52–57
│   └── choose→explore→un-choose; subsets/perms/combos; N-Queens ⭐
│
├── 11. DYNAMIC PROGRAMMING ⭐⭐ ───────────── Days 74–90
│   ├── Ladder: recursion → memo → tabulation → space opt
│   ├── 1D: stairs, house robber, jump game
│   ├── 2D: 0/1 knapsack ⭐, LCS ⭐, edit distance, grids, MCM
│   ├── Strings: LPS, word break
│   └── DP on trees/graphs, bitmask (advanced)
│
├── 12. GREEDY ────────────────────────────── Days 70–73
│   └── Activity selection, jump game, gas station, intervals
│
├── 13. ADVANCED / MISC ───────────────────── Days 91–95
│   └── Bit manipulation, Tries, Two Heaps, number theory
│
└── 14. PRACTICE SYSTEM ───────────────────── Days 96–100
    └── Timed mocks: 4 Medium + 1 Hard/day, spaced revision
```

---

## C++ CORE CONCEPTS YOU'LL LEARN ALONG THE WAY

| Phase | C++ Topic | What you'll use daily |
|---|---|---|
| Foundations | `iostream`, `bits/stdc++.h`, `main()`, compile & run | every single day |
| Arrays | `vector<int>`, `v.push_back()`, `v.size()`, range-for loop, `sort()`, `reverse()`, `pair`, `auto` | Days 4–14 |
| Strings | `string`, `s[i]`, `substr()`, `sort(s.begin(), s.end())`, `unordered_map` for frequency | Days 15–19 |
| Linked List | `struct Node {int val; Node* next;};`, pointers `*`, `->`, `new`/`delete`, `nullptr` | Days 20–26 |
| Stack/Queue | `stack<int>`, `queue<int>`, `deque<int>`, `priority_queue<int>` | Days 27–32 |
| Binary Search | `lower_bound()`, `upper_bound()`, `mid = lo + (hi-lo)/2` (overflow-safe) | Days 33–36 |
| Trees | recursion depth, `struct TreeNode`, DFS with call stack, `queue` for BFS | Days 37–47 |
| Heap | `priority_queue<int, vector<int>, greater<int>>` for min-heap | Days 48–51 |
| Graphs | `vector<vector<int>> adj`, `vector<bool> visited`, `queue<pair<int,int>>`, `const int INF` | Days 58–69 |
| Backtracking | pass-by-reference `&`, backtrack undo step, `vector<vector<int>>` result | Days 52–57 |
| DP | 1D/2D `vector` tables, `INT_MIN`/`INT_MAX`, `max()`/`min()`, space optimization | Days 74–90 |
| Misc | bit ops `& | ^ << >>`, `__builtin_popcount`, `unordered_set`, `tuple` | Days 91–95 |

---

## DAY-BY-DAY SCHEDULE

### Phase 0 — Foundations (Days 1–3)
| Day | Problems | C++ focus |
|---|---|---|
| 1 | 217 Contains Duplicate, 53 Maximum Subarray | `vector`, `sort()`, `unordered_set` |
| 2 | 152 Max Product Subarray, 153 Min in Rotated Array | loops, `INT_MIN`/`INT_MAX` |
| 3 | 15 3Sum, 121 Buy & Sell Stock | two pointers, nested loops |

### Phase 1 — Arrays (Days 4–14)
| Day | Problems | Pattern |
|---|---|---|
| 4 | 1 Two Sum, 268 Missing Number | hashing |
| 5 | 11 Container With Most Water, 167 Two Sum II | two ptr opposite ends |
| 6 | 125 Valid Palindrome, 344 Reverse String | two ptr basics |
| 7 | 26 Remove Duplicates, 283 Move Zeroes | same-direction ptrs |
| 8 | 209 Min Subarray Sum, 643 Max Avg Subarray I | fixed window |
| 9 | 3 Longest Substring No Repeat, 567 Permutation in String | variable window |
| 10 | 424 Longest Repeating Char Replacement, 438 Anagrams | window + hash |
| 11 | ⭐239 Sliding Window Max, ⭐76 Min Window Substring | monotonic queue, hard window |
| 12 | 560 Subarray Sum Equals K, 974 Subarrays Div by K | prefix sum + hash |
| 13 | 75 Sort Colors, 56 Merge Intervals | Dutch flag, sweep |
| 14 | 57 Insert Interval, 33 Search Rotated Array | intervals, rotated BS |
| — | REVISION ⏪ | — |

### Phase 2 — Strings + Hashing (Days 15–19)
| Day | Problems | Pattern |
|---|---|---|
| 15 | 242 Valid Anagram, 49 Group Anagrams | `unordered_map` |
| 16 | 20 Valid Parentheses, 🔒271 Encode/Decode | stack intro |
| 17 | 347 Top K Frequent, 128 Longest Consecutive | bucket, hash |
| 18 | 5 Longest Palindromic Substring, 647 Palindromic Substrings | expand center |
| 19 | REVISION ⏪ | — |

### Phase 3 — Linked List (Days 20–26)
| Day | Problems | Pattern |
|---|---|---|
| 20 | 206 Reverse LL, 141 LL Cycle | ptr manipulation |
| 21 | 142 Cycle II, 876 Middle of LL | fast/slow |
| 22 | 21 Merge 2 Sorted, ⭐23 Merge K Sorted | dummy node, heap |
| 23 | 19 Remove Nth From End, 237 Delete Node | fast/slow + gap |
| 24 | 143 Reorder List, 234 Palindrome LL | reverse + merge |
| 25 | 138 Copy Random Ptr, ⭐146 LRU Cache | hash + DLL |
| 26 | REVISION ⏪ | — |

### Phase 4 — Stack & Queue (Days 27–32)
| Day | Problems | Pattern |
|---|---|---|
| 27 | 155 Min Stack, 150 Eval RPN | aux stack |
| 28 | 22 Generate Parentheses, 739 Daily Temperatures | stack + backtrack |
| 29 | ⭐84 Largest Rectangle, ⭐85 Maximal Rectangle | monotonic stack |
| 30 | 503 Next Greater II, 496 Next Greater I | circular mono stack |
| 31 | 225 Stack via Queues, 232 Queue via Stacks | implementation |
| 32 | REVISION ⏪ | — |

### Phase 5 — Binary Search Deep (Days 33–36)
| Day | Problems | Pattern |
|---|---|---|
| 33 | 704 Binary Search, 35 Search Insert | classic BS |
| 34 | 852 Peak Index, 162 Find Peak | BS on unsorted pattern |
| 35 | 1011 Ship Packages, ⭐410 Split Array Largest Sum | BS on answer |
| 36 | ⭐4 Median 2 Sorted, 81 Search Rotated II | partition BS |

### Phase 6 — Trees (Days 37–47)
| Day | Problems | Pattern |
|---|---|---|
| 37 | 104 Max Depth, 100 Same Tree | basic recursion |
| 38 | 226 Invert Tree, 101 Symmetric Tree | DFS |
| 39 | 102 Level Order, 107 Level Order II | BFS |
| 40 | 98 Validate BST, 235 LCA of BST | BST props |
| 41 | 236 LCA of BT, ⭐297 Serialize/Deserialize | recursion returns |
| 42 | ⭐124 Max Path Sum, 543 Diameter | global var + DFS |
| 43 | 110 Balanced, 199 Right Side View | height, BFS last |
| 44 | 230 Kth Smallest BST, 700 Search BST | inorder |
| 45 | 701 Insert BST, 450 Delete BST | BST surgery |
| 46 | 958 Complete BT, 114 Flatten to LL | BFS check, Morris idea |
| 47 | REVISION ⏪ | — |

### Phase 7 — Heap (Days 48–51)
| Day | Problems | Pattern |
|---|---|---|
| 48 | 703 Kth Largest Stream, 215 Kth Largest | min-heap k size |
| 49 | 973 K Closest Points, 621 Task Scheduler | heap + greedy |
| 50 | ⭐295 Median of Stream, 355 Design Twitter | two heaps |
| 51 | 373 K Pairs Smallest Sums + REVISION | heap + BS hybrid |

### Phase 8 — Backtracking (Days 52–57)
| Day | Problems | Pattern |
|---|---|---|
| 52 | 78 Subsets, 90 Subsets II | include/exclude |
| 53 | 46 Permutations, 47 Permutations II | swap / used[] |
| 54 | 39 Combination Sum, 40 Combination Sum II | remain target |
| 55 | 17 Phone Combos, 79 Word Search | grid DFS |
| 56 | ⭐51 N-Queens, ⭐37 Sudoku Solver | constraint + prune |
| 57 | 131 Palindrome Partitioning + REVISION | prefix check |

### Phase 9 — Graphs (Days 58–69) ⭐
| Day | Problems | Pattern |
|---|---|---|
| 58 | ⭐200 Number of Islands, 695 Max Area | grid DFS |
| 59 | 133 Clone Graph, 733 Flood Fill | BFS/DFS clone |
| 60 | 994 Rotting Oranges, 417 Pacific Atlantic | multi-source BFS |
| 61 | ⭐207 Course Schedule, 210 Course Schedule II | topo sort |
| 62 | ⭐127 Word Ladder, 🔒286 Walls & Gates | BFS shortest |
| 63 | 743 Network Delay, 787 Cheapest Flights K Stops | Dijkstra, Bellman-Ford |
| 64 | 1584 Min Cost Points (Prim's), 684 Redundant (Union-Find) | MST |
| 65 | 721 Accounts Merge, 1319 Connect Network | Union-Find ⭐ |
| 66 | ⭐1192 Critical Connections, 802 Safe States | bridges, reverse topo |
| 67 | 332 Reconstruct Itinerary, 399 Evaluate Division | Euler path, weighted graph |
| 68 | 785 Bipartite, 886 Possible Bipartition | 2-color BFS |
| 69 | REVISION ⏪ | — |

### Phase 10 — Greedy (Days 70–73)
| Day | Problems | Pattern |
|---|---|---|
| 70 | 455 Assign Cookies, 435 Non-overlapping Intervals | sort + greedy |
| 71 | 452 Min Arrows, 55 Jump Game | interval greedy |
| 72 | 45 Jump Game II, 134 Gas Station | range greedy |
| 73 | 135 Candy + REVISION | two-pass greedy |

### Phase 11 — Dynamic Programming (Days 74–90) ⭐⭐
| Day | Problems | Pattern |
|---|---|---|
| 74 | 70 Climbing Stairs, 198 House Robber | 1D memo |
| 75 | 213 House Robber II, 746 Min Cost Stairs | circular 1D |
| 76 | 62 Unique Paths, 63 Unique Paths II | grid DP |
| 77 | 64 Min Path Sum, 120 Triangle | grid DP |
| 78 | 416 Partition Equal Subset, 494 Target Sum | 0/1 knapsack |
| 79 | 518 Coin Change II, 322 Coin Change | unbounded knapsack |
| 80 | ⭐1143 LCS, 583 Delete for 2 Strings | LCS family |
| 81 | ⭐72 Edit Distance, 712 Min ASCII Delete | LCS variant |
| 82 | ⭐300 LIS, 673 Number of LIS | LIS family |
| 83 | 516 LPS | string DP |
| 84 | 139 Word Break, 140 Word Break II | partition DP |
| 85 | 376 Wiggle, 91 Decode Ways | 1D variants |
| 86 | ⭐32 Longest Valid Parens, ⭐42 Trapping Rain Water | stack/two-ptr DP |
| 87 | 221 Maximal Square | 2D DP |
| 88 | ⭐312 Burst Balloons, ⭐10 Regex Matching | interval DP |
| 89 | 115 Distinct Subseq, 44 Wildcard Matching | string DP hard |
| 90 | 188 Stock IV + FULL REVISION ⏪ | state DP |

### Phase 12 — Advanced (Days 91–95)
| Day | Problems | Pattern |
|---|---|---|
| 91 | 208 Trie, 211 Add & Search Words | trie |
| 92 | 212 Word Search II, 421 Max XOR | trie + backtrack |
| 93 | 136 Single Number, 191 Number of 1 Bits | XOR tricks |
| 94 | 190 Reverse Bits, 338 Counting Bits | bit DP |
| 95 | 7 Reverse Integer, 380 Insert Delete GetRandom | design |

### Phase 13 — Mocks (Days 96–100)
- 4 random Medium + 1 Hard per day, 90-min timer
- Re-solve everything you failed earlier

---

## SPACED REVISION RULE
After solving a problem, re-solve it: **Day +3 → Day +7 → Day +30**.
Mark: ✅ solved solo | 🟡 needed hint | 🔴 needed solution
