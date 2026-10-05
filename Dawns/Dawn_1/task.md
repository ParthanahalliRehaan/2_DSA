# Today's Quest: The Handshake Puzzle 🤝

## Part 1: Notebook math (no code, pen and paper only)

**The story:** 6 friends stand in a line, each holding a card: `[3, 8, 5, 1, 9, 4]`. A wizard says: *"Two of you must team up so your cards add to exactly 12."*

Solve these in your notebook:

1. **List every possible pair** (by index) and write each sum. How many pairs are there? Try to find the formula for *n* friends without counting on your fingers (hint: handshakes).
2. **Which pair(s) add to 12?** Write down the indices, not just the values.
3. **Spot the pattern:** for the friend holding `3`, what exact number must their partner hold? Write that "needed partner" next to every friend's card in a second row. What do you notice about the table you just made?
4. **Scale it up:** if there were 1,000 friends, how many pairs would you have checked in step 1? How many "needed partner" lookups would step 3 take? Which one grows faster?
5. **Bonus twist:** the cards are now sorted: `[1, 3, 4, 5, 8, 9]`. Target is still 12. Without listing all pairs, can you find the answer by putting one finger at each end of the line and moving them? Write down the rule you used for "which finger moves?"

Spend 15 to 20 minutes on this. The goal is to *feel* the difference between your approaches before you code anything.

---

## Part 2: The matching LeetCode problem

**LeetCode 167: Two Sum II, Input Array Is Sorted** (Medium, but friendly)

Why this one: it's exactly your wizard puzzle (step 5 in particular), with 1-indexed output and a stricter space requirement.

**Stretch (optional):** Codeforces **1676B/…** is not needed today. If you want a Codeforces warm-up, try **Watermelon (4A)**. It's a tiny pure-math problem that trains the "think on paper first" habit.

---

## Your flow today
1. Solve Part 1 in the notebook.
2. Write 2 to 3 lines: *"my approach was ___, it takes about ___ steps for n friends."*
3. Then code LeetCode 167 in C++ and come back to show me your notebook insights and code. I'll review, but I won't hand you the solution. 😄
