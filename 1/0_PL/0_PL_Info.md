**vocabulary layer**, not the programming layer.

Most college notes assume you already know terms like *static typing*, *compiled*, *paradigm*, *runtime*, *event-driven*, etc. That's like teaching someone to drive while assuming they already know what a clutch is. Admirably optimistic, if slightly detached from reality.

I'd add this **before** the language comparison.

````md
# Programming Language Fundamentals (Must Know)

Before comparing programming languages, understand these common terms.

---

# 1. What is a Programming Paradigm?

A **Programming Paradigm** is simply a **style or way of writing programs**.

Think of it like different ways to build a house.

```
Problem

   │

   ▼

Many Ways to Solve

   │

   ├── Procedural
   ├── Object-Oriented
   ├── Functional
   ├── Event-Driven
   └── Concurrent
```

A language can support **one or many paradigms**.

---

# 2. Procedural Programming (SOP)

Programs are divided into **functions (procedures)**.

Focus:

```
Step 1

↓

Step 2

↓

Step 3

↓

Result
```

Example

```c
main()
{
    read();
    calculate();
    print();
}
```

Languages

- C
- Go
- C++ (also supports OOP)

Best for

- Small programs
- Fast execution
- System software

---

# 3. Object-Oriented Programming (OOP)

Everything revolves around **Objects**.

Instead of asking

> What should happen next?

You ask

> Which object should do this?

Example

```
Car

│

├── Start()

├── Stop()

└── Brake()
```

Concepts

- Class
- Object
- Encapsulation
- Inheritance
- Polymorphism
- Abstraction

Languages

- Java
- C++
- Python
- JavaScript
- TypeScript

---

# 4. Functional Programming

Programs are built using **functions**.

Rules

- Avoid changing variables
- Avoid global state
- Same input → Same output

Example

```
square(5)

↓

25
```

Languages

- Python
- JavaScript
- Rust
- Scala
- Haskell

---

# 5. Event-Driven Programming

Program waits until **an event happens**.

Examples of events

- Mouse Click
- Keyboard Press
- Button Click
- Network Request
- Timer
- File Download

```
Program Starts

↓

Wait...

↓

User Clicks Button

↓

Run Function
```

Example

```javascript
button.onclick = function()
{
    alert("Hello");
}
```

JavaScript became famous because web pages constantly react to events.

Other languages **can** do event-driven programming too (Java, C#, Python), but JavaScript is designed around it and uses it everywhere in browsers.

---

# 6. Concurrent Programming

Multiple tasks make progress at the same time.

Example

A browser can

```
Download File

+

Play Music

+

Render Webpage

+

Accept Mouse Clicks
```

all without waiting for one another.

Languages

- Go ⭐⭐⭐⭐⭐
- Rust ⭐⭐⭐⭐☆
- Java ⭐⭐⭐⭐☆
- C++ ⭐⭐⭐☆
- Python ⭐⭐☆

---

# 7. What is Typing?

Typing means

**How a language handles variable data types.**

Example

```
10

Integer

"A"

String

3.14

Float
```

---

# Static Typing

Type is fixed before the program runs.

Compiler checks everything.

Example (Java)

```java
int age = 20;
```

Cannot do

```java
age = "Hello";
```

Error occurs **before running**.

Advantages

- Fewer bugs
- Faster execution
- Better optimization

Languages

- C
- C++
- Java
- Go
- Rust
- TypeScript

---

# Dynamic Typing

Type is decided while the program runs.

Example (Python)

```python
x = 10
```

Later

```python
x = "Hello"
```

Perfectly valid.

Advantages

- Easy to write
- Flexible

Disadvantages

- More runtime errors
- Slightly slower

Languages

- Python
- JavaScript

---

# 8. Compiler

A Compiler translates the **entire program** before execution.

```
Source Code

↓

Compiler

↓

Machine Code

↓

Run
```

Advantages

- Very fast execution
- Errors found before running

Examples

- C
- C++
- Rust
- Go

---

# 9. Interpreter

Reads and executes code step-by-step.

```
Read Line

↓

Execute

↓

Read Next Line

↓

Execute
```

Advantages

- Easy debugging
- Fast development

Disadvantages

- Slower execution

Example

Python

---

# 10. JIT (Just-In-Time Compiler)

A mixture of compilation and interpretation.

```
Program Starts

↓

Interpreter

↓

Frequently Used Code

↓

Compiled into Machine Code

↓

Runs Faster
```

Used by

- Java
- JavaScript

---

# 11. Bytecode

Bytecode is an **intermediate language**.

```
Java Source

↓

Bytecode

↓

JVM

↓

Machine Code
```

It is **not machine code**.

It is also **not source code**.

It sits in between.

---

# 12. Virtual Machine (VM)

A Virtual Machine acts like a computer inside your computer.

Example

```
Java Program

↓

Java Virtual Machine

↓

Windows

Linux

macOS
```

Because every OS has a JVM,

Java becomes

```
Write Once

Run Anywhere
```

---

# 13. Runtime

Runtime simply means

> The period when your program is actually executing.

Example

```
Compile

↓

Run

← This is Runtime
```

Errors during runtime are called **Runtime Errors**.

---

# 14. Garbage Collection (GC)

Automatically removes unused memory.

Without GC

```
Programmer

↓

Allocate Memory

↓

Free Memory
```

With GC

```
Programmer

↓

Allocate Memory

↓

Garbage Collector cleans automatically
```

Languages

- Java
- Go
- Python
- JavaScript

No Garbage Collector

- C
- C++
- Rust (uses Ownership instead)

---

# 15. Ownership (Rust)

Rust does not use Garbage Collection.

Instead,

Every piece of memory has exactly one owner.

```
Memory

↓

Owner Variable

↓

Owner disappears

↓

Memory freed automatically
```

No leaks.

No Garbage Collector.

Very efficient.

---

# Language Comparison

| Language | Main Paradigm | Event Driven | Typing | Execution | Memory | Best Applications |
|-----------|---------------|--------------|---------|-----------|--------|-------------------|
| C | Procedural | ❌ | Static | Compiled | Manual | OS, Drivers, Embedded Systems |
| C++ | Multi-Paradigm | ❌ | Static | Compiled | Manual / Smart Pointers | Games, Graphics, Finance |
| Rust | Systems + Functional | ❌ | Static | Compiled | Ownership | Secure Systems, OS, Servers |
| Go | Procedural + Concurrent | ❌ | Static | Compiled | Garbage Collection | Cloud, APIs, Kubernetes |
| Java | OOP + Functional | Limited | Static | Bytecode + JVM + JIT | Garbage Collection | Enterprise, Banking, Android |
| Python | Multi-Paradigm | Supported | Dynamic | Interpreted | Garbage Collection | AI, ML, Automation, Data Science |
| JavaScript | Event-Driven + Functional + OOP | ✅ Native | Dynamic | JIT | Garbage Collection | Websites, Frontend, Node.js |
| TypeScript | JavaScript + Static Types | ✅ Native | Static (Compile Time) | Transpiles → JavaScript | Garbage Collection | Large Web Applications |

---

# One-Line Memory Tricks

```
Procedural
→ Do this, then this, then this.

OOP
→ Objects do the work.

Functional
→ Solve using pure functions.

Event-Driven
→ Wait for an event, then react.

Concurrent
→ Many tasks progress together.

Static Typing
→ Type fixed before running.

Dynamic Typing
→ Type decided while running.

Compiled
→ Translate everything first.

Interpreted
→ Translate while executing.

JIT
→ Compile only frequently used code.

Bytecode
→ Intermediate code.

Runtime
→ Program is currently running.

Garbage Collection
→ Automatic memory cleanup.

Ownership
→ Rust's compile-time memory management.
```
````

This vocabulary sheet is honestly more valuable than memorizing language names. Once these 15-20 terms click, almost every "why is language X different from language Y?" question becomes much easier to answer instead of feeling like random facts.
