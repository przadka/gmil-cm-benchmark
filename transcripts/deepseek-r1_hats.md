<USER>
### 8. Hats

Pola has a pair of plush monsters: a three-headed Cerberus and a two-headed Dragon. She really enjoys playing with these plush toys by putting hats on their heads. Pola has four identical white hats, two identical green hats, and one red hat. It is known that each of these hats can be placed on any head of Cerberus or the Dragon.

**In how many different ways can Pola put the hats on her plush toys so that each head has exactly one hat?**  
Two ways of putting on the hats are considered different if the hats on at least one head of one of the plush toys are of different colors.

<ASSISTANT>
### Understanding the Problem

First, let's break down the problem to understand all its components:

- **Plush Monsters:**
  - **Cerberus:** A three-headed monster.
  - **Dragon:** A two-headed monster.
  
- **Hats Available:**
  - **4 identical white hats**
  - **2 identical green hats**
  - **1 red hat**
  
- **Total Heads to Cover:** 3 (Cerberus) + 2 (Dragon) = **5 heads**

- **Objective:** Determine the number of distinct ways to place the hats on the heads such that each head has exactly one hat. Two arrangements are considered different if at least one head has a hat of a different color.

### Initial Thoughts

Since each head must have exactly one hat, and we have a total of 5 heads, we need to distribute the 7 hats (4 white + 2 green + 1 red) onto these 5 heads. However, since there are more hats than heads, some hats will remain unused. But the problem specifies that each head must have exactly one hat, implying that exactly 5 hats will be used, and 2 hats will be left out.

Given that, we need to:

1. **Select 5 hats out of the 7 available.**
2. **Distribute these 5 hats onto the 5 heads, considering the colors.**

But wait, the hats of the same color are identical. This means that the arrangement depends on the number of hats of each color used, not on which specific hat is used.

### Step 1: Selecting 5 Hats from 7

We have:

- 4 white hats
- 2 green hats
- 1 red hat

We need to choose 5 hats in total. Let's consider the possible combinations of colors:

1. **All 4 white hats + 1 green hat:** Total = 5 hats
2. **All 4 white hats + 1 red hat:** Total = 5 hats
3. **3 white hats + 2 green hats:** Total = 5 hats
4. **3 white hats + 1 green hat + 1 red hat:** Total = 5 hats
5. **2 white hats + 2 green hats + 1 red hat:** Total = 5 hats

These are the possible ways to select 5 hats from the available pool.

### Step 2: Distributing the Selected Hats onto the Heads

Now, for each selection of 5 hats, we need to determine how many distinct ways we can distribute them onto the 5 heads.

Since the hats of the same color are identical, the arrangement depends on how many heads get each color.

Let's analyze each case:

#### Case 1: 4 White Hats + 1 Green Hat

- **Colors to distribute:** 4 white, 1 green
- **Total heads:** 5

We need to choose which head gets the green hat. The rest will automatically get white hats.

- **Number of ways:** C(5,1) = 5

#### Case 2: 4 White Hats + 1 Red Hat

- **Colors to distribute:** 4 white, 1 red
- **Total heads:** 5

Similar to Case 1, we choose which head gets the red hat.

- **Number of ways:** C(5,1) = 5

#### Case 3: 3 White Hats + 2 Green Hats

- **Colors to distribute:** 3 white, 2 green
- **Total heads:** 5

We need to choose which 2 heads get the green hats. The rest will get white hats.

- **Number of ways:** C(5,2) = 10

#### Case 4: 3 White Hats + 1 Green Hat + 1 Red Hat

- **Colors to distribute:** 3 white, 1 green, 1 red
- **Total heads:** 5

We need to choose:

1. Which head gets the green hat.
2. Which head gets the red hat.
3. The remaining heads get white hats.

- **Number of ways:** C(5,1) for green * C(4,1) for red = 5 * 4 = 20

Wait, let's verify this:

After assigning the green hat to one head, there are 4 heads left for the red hat.

So, total ways = 5 (green) * 4 (red) = 20

#### Case 5: 2 White Hats + 2 Green Hats + 1 Red Hat

- **Colors to distribute:** 2 white, 2 green, 1 red
- **Total heads:** 5

We need to choose:

1. Which 2 heads get the green hats.
2. Which 1 head gets the red hat.
3. The remaining heads get white hats.

- **Number of ways:** C(5,2) for green * C(3,1) for red = 10 * 3 = 30

Let's verify:

First, choose 2 heads out of 5 for green hats: C(5,2) = 10

Then, choose 1 head out of the remaining 3 for the red hat: C(3,1) = 3

Total ways = 10 * 3 = 30

### Summing Up All Cases

Now, we'll add up the number of ways from all cases:

1. **Case 1:** 5 ways
2. **Case 2:** 5 ways
3. **Case 3:** 10 ways
4. **Case 4:** 20 ways
5. **Case 5:** 30 ways

**Total number of ways = 5 + 5 + 10 + 20 + 30 = 70**

### Verification

To ensure that we haven't missed any cases or overcounted, let's revisit our initial selection of hats:

- We considered all possible combinations where the total number of hats is 5, using the available counts of each color.
- Each case was distinct in terms of the number of hats of each color used.
- The distribution calculations for each case correctly accounted for the identical nature of hats of the same color.

Therefore, the total number of distinct ways Pola can put the hats on her plush toys is **70**.

### Final Answer

**There are 70 different ways Pola can put the hats on her plush toys so that each head has exactly one hat.**