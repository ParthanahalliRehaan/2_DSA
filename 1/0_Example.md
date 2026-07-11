## Side Note: Why We Ignore Small Inputs

Suppose two algorithms solve the same problem.

- **Algorithm A** → Exponential `O(2ⁿ)`
- **Algorithm B** → Linear `O(n)`

At **small inputs**, Algorithm A may actually appear faster because it has very little overhead.

| Input Size (n) | Algorithm A (Exponential) | Algorithm B (Linear) |
|---------------:|--------------------------:|---------------------:|
| 5              | 1 sec                     | 30 sec               |
| 10             | 5 sec                     | 60 sec               |
| 20             | 80 sec                    | 120 sec              |
| 30             | 5,000 sec                 | 180 sec              |
| 40             | 1,000,000+ sec            | 240 sec              |

### Observation

Initially:

```
Algorithm A < Algorithm B
```

As input grows:

```
Algorithm A >>>>>>>>>>> Algorithm B
```

This is why Computer Science focuses on **growth rate**, not initial execution time.

A slower algorithm at small inputs may become **far superior** for large inputs if it has a lower time complexity.

Example:

```
A : O(2ⁿ)
B : O(n)

Small n:
A is faster

Large n:
B completely dominates A
```

**Key Takeaway**

> Never judge an algorithm using only one small test case. Always analyze how it scales as the input size (`n`) increases.