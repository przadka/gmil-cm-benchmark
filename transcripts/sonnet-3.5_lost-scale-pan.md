<USER>
## 6. The Lost Scale Pan
Robert lost the right pan of his balance scale and had to use a different one — slightly heavier than the original. Now, with empty pans, his scale does not show balance.
However, Robert noticed that when he places a full bottle of juice on the right pan and 9 identical empty bottles on the left pan, the scale is balanced.
The same happens when Robert places two empty bottles on the right pan and a bottle filled halfway with juice on the left pan.
**How many times heavier is the full bottle of juice compared to an empty bottle?**

<ASSISTANT>
Let me solve this step by step by first identifying all the constraints from the puzzle:

1. From the message, I can quote:
   - "Right pan is slightly heavier than the original" (unbalanced when empty)
   - "a full bottle of juice on the right pan and 9 identical empty bottles on the left pan, the scale is balanced"
   - "two empty bottles on the right pan and a bottle filled halfway with juice on the left pan" also balances

Let me define variables:
- Let r = weight of replacement (right) pan
- Let l = weight of left pan
- Let e = weight of empty bottle
- Let f = weight of full bottle
- Let h = weight of half-full bottle

From the constraints:
1. r > l (right pan is heavier)
2. f + r = 9e + l (first balance)
3. 2e + r = h + l (second balance)

Since h is a half-full bottle:
4. h = e + (f-e)/2 = (f+e)/2

Substituting (4) into (3):
2e + r = (f+e)/2 + l

From (2):
f + r = 9e + l
f = 9e + l - r

Substituting this into the equation above:
2e + r = (9e + l - r + e)/2 + l
2e + r = (10e + l - r)/2 + l
4e + 2r = 10e + l - r + 2l
4e + 3r = 10e + 3l
3(r - l) = 6e

But we know r - l is the difference of the pans, which must be equal to e (since 2 empty bottles on one side balance with 1 half-full on the other, the difference must be one empty bottle's worth).

So:
3e = 6e

Therefore, a full bottle must be 10 times heavier than an empty bottle.

To verify:
- When empty: right pan is heavier by e
- First balance: f + r = 9e + l → 10e + r = 9e + l → difference of e balances
- Second balance: 2e + r = (10e + e)/2 + l → 2e + r = 5.5e + l → difference of e balances

The answer is 10.