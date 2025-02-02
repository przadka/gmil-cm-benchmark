<USER>
### 8. Hats

Pola has a pair of plush monsters: a three-headed Cerberus and a two-headed Dragon. She really enjoys playing with these plush toys by putting hats on their heads. Pola has four identical white hats, two identical green hats, and one red hat. It is known that each of these hats can be placed on any head of Cerberus or the Dragon.

**In how many different ways can Pola put the hats on her plush toys so that each head has exactly one hat?**  
Two ways of putting on the hats are considered different if the hats on at least one head of one of the plush toys are of different colors.

<ASSISTANT>
We wish to assign a hat (of a given color) to each of the 5 distinct heads (3 on Cerberus and 2 on the Dragon). The hats come in three colors, but with limited supply:
- **White:** 4 hats
- **Green:** 2 hats
- **Red:** 1 hat

An assignment is just a way to choose a color for each head so that:
- The number of white hats used is at most 4.
- The number of green hats used is at most 2.
- The number of red hats used is at most 1.
- And every head gets exactly one hat.

We can think of such an assignment by letting \(w\), \(g\), and \(r\) be the number of white, green, and red hats used, respectively. Since there are 5 heads, we have
\[
w+g+r=5,
\]
with the restrictions:
\[
w\le4,\quad g\le2,\quad r\le1.
\]

We now consider the two possible cases for \(r\): either \(r=0\) or \(r=1\).

---

### **Case 1. \(r=0\) (No red hat is used)**

Then, \(w+g=5\) with the conditions:
- \(w\le4\) (so \(w=5\) is not allowed), and
- \(g\le2\).

The possible pairs \((w, g)\) are:
1. \(w=4\) and \(g=1\)  
2. \(w=3\) and \(g=2\)

Now, count the assignments:

1. **\(w=4, g=1\):**  
   - Choose 4 heads (out of 5) to receive white hats. The remaining head will receive a green hat.  
   - Number of ways: \(\binom{5}{4}=5\).

2. **\(w=3, g=2\):**  
   - Choose 3 heads (out of 5) to receive white hats. The remaining 2 heads receive green hats.  
   - Number of ways: \(\binom{5}{3}=10\).

Thus, the total for \(r=0\) is:
\[
5+10=15.
\]

---

### **Case 2. \(r=1\) (The red hat is used on one head)**

Now, with one red hat used, the remaining hats must cover 4 heads:
\[
w+g=4,
\]
with the same limits: \(w\le4\) and \(g\le2\).

The possible splits are:
1. \(w=4\) and \(g=0\)
2. \(w=3\) and \(g=1\)
3. \(w=2\) and \(g=2\)

Count the assignments step by step:

1. **\(w=4, g=0\):**  
   - First, choose which head gets the red hat: \(\binom{5}{1}=5\) ways.  
   - The remaining 4 heads all get white hats (only 1 way to do this).  
   - Total ways: \(5 \times 1 = 5\).

2. **\(w=3, g=1\):**  
   - Choose the head for the red hat: \(\binom{5}{1}=5\) ways.  
   - For the remaining 4 heads, choose 3 to get white hats (the other gets a green hat): \(\binom{4}{3}=4\) ways.  
   - Total ways: \(5 \times 4 = 20\).

3. **\(w=2, g=2\):**  
   - Choose the red hat head: \(\binom{5}{1}=5\) ways.  
   - For the remaining 4 heads, choose 2 to receive white hats (the other 2 get green hats): \(\binom{4}{2}=6\) ways.  
   - Total ways: \(5 \times 6 = 30\).

Thus, the total for \(r=1\) is:
\[
5+20+30=55.
\]

---

### **Final Count**

Adding the results from both cases:
\[
15\ (\text{for } r=0) + 55\ (\text{for } r=1) = 70.
\]

So, there are **70 different ways** for Pola to put the hats on her plush toys so that each head has exactly one hat.

\[
\boxed{70}
\]