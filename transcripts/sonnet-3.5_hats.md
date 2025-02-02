<USER>
### 8. Hats
Pola has a pair of plush monsters: a three-headed Cerberus and a two-headed Dragon. She really enjoys playing with these plush toys by putting hats on their heads. Pola has four identical white hats, two identical green hats, and one red hat. It is known that each of these hats can be placed on any head of Cerberus or the Dragon.
**In how many different ways can Pola put the hats on her plush toys so that each head has exactly one hat?**  
Two ways of putting on the hats are considered different if the hats on at least one head of one of the plush toys are of different colors.

<ASSISTANT>
Let me solve this step by step.

First, let me identify the key constraints from the problem:

1. From "Pola has a pair of plush monsters: a three-headed Cerberus and a two-headed Dragon"
- Cerberus has 3 heads
- Dragon has 2 heads
- Total of 5 heads need hats

2. From "Pola has four identical white hats, two identical green hats, and one red hat"
- 4 white hats (identical)
- 2 green hats (identical)
- 1 red hat
- Total of 7 hats available

3. From "each head has exactly one hat"
- All 5 heads must get exactly one hat
- We must use exactly 5 hats out of the 7 available

4. From "Two ways of putting on the hats are considered different if the hats on at least one head of one of the plush toys are of different colors"
- Since hats of same color are identical, we only care about the color pattern

Let me solve this using the distribution method:
1) First, let's consider how many red hats we'll use (0 or 1, since we only have 1)
2) Then for each case, we'll consider how many green hats we'll use (0, 1, or 2, since we have 2)
3) The remaining heads will get white hats

Case 1: Using 0 red hats
- Using 0 green hats: WWWWW (1 way)
- Using 1 green hat: GWWWW (5 choose 1 = 5 ways)
- Using 2 green hats: GGWWW (5 choose 2 = 10 ways)

Case 2: Using 1 red hat
- Using 0 green hats: RWWWW (5 choose 1 = 5 ways)
- Using 1 green hat: RGWWW (5 choose 1 × 4 choose 1 = 20 ways)
- Using 2 green hats: RGGWW (5 choose 1 × 4 choose 2 = 30 ways)

Total number of ways = 1 + 5 + 10 + 5 + 20 + 30 = 71

The answer is 71 different ways.

To verify this solution:
- We've considered all possible color combinations
- Each combination uses 5 hats total (matching number of heads)
- We never used more hats than available of each color
- The combinations are distinct since changing position of same-colored hats doesn't create a new combination
- We've accounted for all possible positions of each color combination