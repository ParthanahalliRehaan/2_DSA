# Module 1: Algorithm Analysis (Complete Notes)

> Exam Survival Guide. Because apparently humans enjoy measuring how slowly computers suffer.

---

# 1. Why Algorithms & Data Structures?

## Algorithm
An algorithm is a finite sequence of well-defined steps to solve a problem.

Example:
```
Input → Process → Output
```

Example:
```
Find Maximum

Read n
max = a[0]

for i = 1 to n-1
    if a[i] > max
        max = a[i]

Print max
```

---

## Data Structure

A method of organizing data efficiently.

Examples:

- Array
- Linked List
- Stack
- Queue
- Tree
- Graph
- Hash Table

Good Data Structures
→ Faster searching
→ Faster insertion
→ Faster deletion
→ Less memory

---

# Why Analyze Algorithms?

Two algorithms may solve the same problem.

Example:

Algorithm A → 1 second

Algorithm B → 30 seconds

As input grows,

Algorithm A
```
100 → 1 sec
1000 → 2 sec
10000 → 4 sec
```

Algorithm B
```
100 → 1 sec
1000 → 40 sec
10000 → 4000 sec
```

Hence,
Efficiency matters more than just correctness.

---

# Performance Depends On

- Input Size (n)
- CPU
- Compiler
- Programming Language
- Algorithm

Algorithm has the biggest impact.

---

# 2. Time Complexity

Measures execution time as input size increases.

NOT actual seconds.

Instead count:

- Comparisons
- Assignments
- Loop executions
- Recursive calls

Example

```
for(i=0;i<n;i++)
    print(i);
```

Runs n times

Time Complexity:

```
O(n)
```

---

# 3. Space Complexity

Measures memory used.

Includes

- Variables
- Arrays
- Recursion Stack
- Dynamic Memory

Example

```
int sum=0;
```

Only one variable

```
Space = O(1)
```

Example

```
int arr[n];
```

Stores n elements

```
Space = O(n)
```

Recursive functions:

Need stack memory.

Example

```
factorial(100)
```

100 recursive calls

```
Space = O(n)
```

---

# Time vs Space

Sometimes

Less Time
↓

More Memory

or

Less Memory
↓

More Time

Tradeoff is common.

---

# 4. Asymptotic Notations

Used to describe algorithm growth.

Three types

- Big O
- Big Theta
- Big Omega

---

# Big O (Worst Case)

Upper Bound

Algorithm never grows faster than this.

Example

```
3n²+5n+10
```

Drop constants

```
O(n²)
```

Graph

```
Time
 ^
 |            O(n²)
 |          /
 |        /
 |      /
 |    /
 |__ /____________> n
```

---

# Big Theta (Average/Tight Bound)

Exact growth.

Upper = Lower

```
Θ(n²)
```

Graph

```
Time
 ^
 |        Θ(n²)
 |      /
 |    /
 |  /
 |/
 +-----------------> n
```

---

# Big Omega (Best Case)

Lower Bound

Minimum work.

Example

Linear Search

Best case

Element found first.

```
Ω(1)
```

Graph

```
Time
 ^
 | O(n)
 |   /
 |  /
 | /
 |/____ Ω(1)
 +-----------------> n
```

---

# Easy Trick

Think of speed limits.

Big O

"Will never exceed"

Big Ω

"Will never go below"

Big Θ

"Exactly around"

---

# 5. Orders of Growth

From fastest to slowest

```
O(1)

↓

O(log n)

↓

O(√n)

↓

O(n)

↓

O(n log n)

↓

O(n²)

↓

O(n³)

↓

O(2ⁿ)

↓

O(n!)
```

Graph

```
Time
^

|                            n!
|                        2^n
|                   n³
|               n²
|          nlogn
|       n
|    logn
| O(1)
+---------------------------------> n
```

---

# Memory Trick

```
1
↓

log n

↓

√n

↓

n

↓

n log n

↓

n²

↓

n³

↓

2ⁿ

↓

n!
```

---

# 6. Best Worst Average Case

Example

Linear Search

```
5 8 2 7 1
```

Search 5

First position

```
Best = O(1)
```

Search 1

Last position

```
Worst = O(n)
```

Random element

```
Average = O(n)
```

---

# Binary Search

Best

```
O(1)
```

Worst

```
O(log n)
```

Average

```
O(log n)
```

---

# 7. Rules for Finding Time Complexity

## Rule 1

Simple statement

```
a=b+c;
```

```
O(1)
```

---

## Rule 2

Loop

```
for(i=0;i<n;i++)
```

Runs n times

```
O(n)
```

---

## Rule 3

Nested loops

```
for(i=0;i<n;i++)
    for(j=0;j<n;j++)
```

```
n*n

O(n²)
```

---

## Rule 4

Consecutive loops

```
for(i=0;i<n;i++)

for(i=0;i<n;i++)
```

```
n+n

O(n)
```

Not O(2n)

Drop constants.

---

## Rule 5

Different limits

```
for(i=0;i<n;i++)

for(j=0;j<m;j++)
```

```
O(n+m)
```

---

## Rule 6

Multiplying loops

```
for(i=0;i<n;i++)

for(j=0;j<m;j++)
```

inside each other

```
O(nm)
```

---

# 8. Complex Loop Examples

---

## Example 1

```
for(i=1;i<=n;i++)
{
    for(j=1;j<=i;j++)
    {
        print();
    }
}
```

Iterations

```
1+2+3+4+...+n

=n(n+1)/2

≈ n²
```

```
TC = O(n²)
SC = O(1)
```

---

## Example 2

```
for(i=n;i>1;i/=2)
```

Values

```
n

n/2

n/4

n/8

...

1
```

Number of divisions

```
log₂n
```

```
TC = O(log n)
```

---

## Example 3

```
for(i=1;i<n;i*=2)
```

Values

```
1

2

4

8

16
```

```
TC = O(log n)
```

---

## Example 4

```
for(i=0;i<n;i++)
{
    for(j=1;j<n;j*=2)
    {
        print();
    }
}
```

Outer

```
n
```

Inner

```
log n
```

Multiply

```
TC = O(n log n)
```

---

## Example 5

```
i=n;

while(i>0)
{
    i=i/3;
}
```

Sequence

```
n

n/3

n/9

n/27

...
```

```
TC = O(log₃ n)

≈ O(log n)
```

---

## Example 6

```
i=1;

while(i<n)
{
    i=i*3;
}
```

```
TC = O(log n)
```

---

## Example 7

```
for(i=1;i<n;i++)
{
    for(j=i;j<n;j++)
    {
        print();
    }
}
```

Iterations

```
n+(n-1)+(n-2)...

=n(n+1)/2

≈ O(n²)
```

---

## Example 8

```
for(i=1;i<n;i*=2)
{
    for(j=1;j<n;j++)
    {
        print();
    }
}
```

Outer

```
log n
```

Inner

```
n
```

```
TC = O(n log n)
```

---

## Example 9

```
for(i=1;i<n;i++)
{
    for(j=1;j<i*i;j++)
    {
        print();
    }
}
```

Inner

```
i²
```

Total

```
1²+2²+3²...

=n(n+1)(2n+1)/6

≈ O(n³)
```

---

## Example 10

```
for(i=1;i<n;i++)
{
    for(j=1;j<n*n;j++)
    {
        print();
    }
}
```

Outer

```
n
```

Inner

```
n²
```

```
O(n³)
```

---

# 9. Recursive vs Non-Recursive Algorithms

## Non Recursive

Uses loops.

Example

```
for()

while()
```

Advantages

- Less memory
- Faster
- No stack overflow

---

## Recursive

Function calls itself.

Example

```
factorial(n)
```

Advantages

- Easy to write
- Cleaner
- Best for Trees

Disadvantages

- More stack memory
- Slightly slower

---

# 10. Recurrence Relations

General form

```
T(n)=Time taken
```

Example

Merge Sort

```
T(n)=2T(n/2)+n
```

---

# Method 1

Iteration Method

Example

```
T(n)=T(n-1)+1
```

Expand

```
=T(n-2)+2

=T(n-3)+3

...

=T(1)+n

O(n)
```

---

Example

```
T(n)=T(n/2)+1
```

Expand

```
=T(n/4)+2

=T(n/8)+3

...

=T(1)+log n

O(log n)
```

---

# Method 2

Substitution Method

Guess

```
T(n)=O(n log n)
```

Substitute.

If equation satisfies

Guess is correct.

Mostly theoretical.

---

# Method 3

Master Method

Formula

```
T(n)=aT(n/b)+f(n)
```

Compare

```
f(n)

with

n^(log_b a)
```

---

Case 1

```
f(n) is smaller
```

Answer

```
O(n^(log_ba))
```

---

Case 2

Equal

```
O(n^(log_ba) log n)
```

---

Case 3

f(n) bigger

```
O(f(n))
```

---

Master Table

| Recurrence | Complexity |
|------------|------------|
| T(n)=2T(n/2)+1 | O(n) |
| T(n)=2T(n/2)+n | O(n log n) |
| T(n)=2T(n/2)+n² | O(n²) |
| T(n)=8T(n/2)+n² | O(n³) |
| T(n)=T(n/2)+1 | O(log n) |
| T(n)=T(n/2)+n | O(n) |

---

# Method 4

Recursion Tree

Example

```
T(n)=2T(n/2)+n
```

Tree

```
            n

      n/2      n/2

   n/4 n/4  n/4 n/4

Each level cost

=n

Levels

=log n

Total

n log n
```

Answer

```
O(n log n)
```

---

# 11. Proof of Correctness

Need to prove algorithm always works.

Methods

- Mathematical Induction
- Loop Invariant

---

## Loop Invariant

Three steps

Initialization

Maintenance

Termination

Example

Finding Maximum

Invariant

```
Before every iteration

max contains largest element seen so far.
```

At end

Largest element found.

Hence algorithm correct.

---

# Quick Time Complexity Cheat Sheet

| Code | TC |
|------|----|
| x=a+b | O(1) |
| for(i=0;i<n;i++) | O(n) |
| while(i>1)i/=2 | O(log n) |
| while(i<n)i*=2 | O(log n) |
| Two nested loops | O(n²) |
| Triple nested loops | O(n³) |
| Half inner loop | O(n²) |
| Outer n Inner logn | O(n log n) |
| Fibonacci Recursive | O(2ⁿ) |
| Binary Search | O(log n) |
| Merge Sort | O(n log n) |
| Quick Sort (Avg) | O(n log n) |
| Quick Sort (Worst) | O(n²) |
| Bubble Sort | O(n²) |
| Selection Sort | O(n²) |
| Insertion Sort (Worst) | O(n²) |

---

# Space Complexity Cheat Sheet

| Code | SC |
|------|----|
| Variables only | O(1) |
| Array of n | O(n) |
| Matrix n×n | O(n²) |
| Recursive depth n | O(n) |
| Recursive depth log n | O(log n) |

---

# Ultimate Shortcuts (Exam Hacks)

## Loop Shortcuts

```
i++

→ O(n)

i+=2

→ O(n)

i*=2

→ O(log n)

i/=2

→ O(log n)

Nested loops

→ Multiply

Consecutive loops

→ Add

1+2+3+...+n

→ O(n²)

1²+2²+...+n²

→ O(n³)

1+1/2+1/4...

→ O(1)
```

---

## Big-O Simplification Rules

```
3n² + 5n + 10
↓

Drop constants

↓

O(n²)
```

```
100n + 500

↓

O(n)
```

```
n² + nlogn + n

↓

O(n²)
```

Only keep the fastest-growing term.

---

# Last-Minute Revision (1 Minute)

- Constant operations → O(1)
- Single loop → O(n)
- Divide/Multiply by constant each iteration → O(log n)
- Nested loops → Multiply
- Consecutive loops → Add
- Triangle loops (1+2+...+n) → O(n²)
- Sum of squares → O(n³)
- Binary Search → O(log n)
- Merge Sort → O(n log n)
- Bubble/Selection/Insertion → O(n²)
- Big O = Worst Case
- Big Ω = Best Case
- Big Θ = Tight Bound
- Recursive algorithms also consume stack space.
- Master Method solves recurrences of the form `T(n)=aT(n/b)+f(n)` quickly.

---
**If you can solve loop complexity, recurrence relations, and Master Method cases confidently, you've covered about 70-80% of the computational questions typically asked in Module 1.**
