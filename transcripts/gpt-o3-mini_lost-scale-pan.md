<USER>
## 6. The Lost Scale Pan

Robert lost the right pan of his balance scale and had to use a different one — slightly heavier than the original. Now, with empty pans, his scale does not show balance.

However, Robert noticed that when he places a full bottle of juice on the right pan and 9 identical empty bottles on the left pan, the scale is balanced.

The same happens when Robert places two empty bottles on the right pan and a bottle filled halfway with juice on the left pan.

**How many times heavier is the full bottle of juice compared to an empty bottle?**

<ASSISTANT>
Let \( E \) be the weight of an empty bottle and \( x \) be the weight of the juice when a bottle is full. Then a full bottle weighs 
\[
F = E + x,
\]
and a bottle that is half-full weighs
\[
E + \frac{x}{2}.
\]

Robert’s scale is unbalanced because his replacement right pan is heavier than the original left pan. We can model the situation by “incorporating” the extra weight of the heavier right pan into our balance equations. Denote:
- \( L \) as the weight of the left pan, and 
- \( R \) as the weight of the right pan (with \( R > L \)).

When objects are placed on the pans, the scale balances if
\[
\text{(left pan weight + its contents)} = \text{(right pan weight + its contents)}.
\]

### The Two Conditions

1. **First Condition:**
   - Left pan: 9 empty bottles (total weight \( 9E \)).
   - Right pan: 1 full bottle (weight \( F = E + x \)).
   
   The balance condition gives:
   \[
   L + 9E = R + (E + x). \tag{1}
   \]

2. **Second Condition:**
   - Left pan: 1 half-full bottle (weight \( E + \frac{x}{2} \)).
   - Right pan: 2 empty bottles (total weight \( 2E \)).
   
   The balance condition gives:
   \[
   L + \left(E + \frac{x}{2}\right) = R + 2E. \tag{2}
   \]

### Eliminating the Unknowns \( L \) and \( R \)

Subtract equation \((2)\) from equation \((1)\) to eliminate \( L \) and \( R \):

\[
\begin{aligned}
\Bigl[L + 9E\Bigr] - \Bigl[L + E + \frac{x}{2}\Bigr] &= \Bigl[R + (E + x)\Bigr] - \Bigl[R + 2E\Bigr] \\
9E - E - \frac{x}{2} &= (E + x) - 2E \\
8E - \frac{x}{2} &= x - E.
\end{aligned}
\]

Multiply both sides of the equation by 2 to eliminate the fraction:

\[
16E - x = 2x - 2E.
\]

Now, solve for \( x \):

\[
\begin{aligned}
16E + 2E &= 2x + x \\
18E &= 3x \\
x &= 6E.
\end{aligned}
\]

### Finding the Ratio

The full bottle weighs
\[
F = E + x = E + 6E = 7E.
\]
Thus, a full bottle is 7 times heavier than an empty bottle.

### Final Answer

The full bottle of juice is **7 times heavier** than the empty bottle.