<USER>
### 8. Hats

Pola has a pair of plush monsters: a three-headed Cerberus and a two-headed Dragon. She really enjoys playing with these plush toys by putting hats on their heads. Pola has four identical white hats, two identical green hats, and one red hat. It is known that each of these hats can be placed on any head of Cerberus or the Dragon.

**In how many different ways can Pola put the hats on her plush toys so that each head has exactly one hat?**  
Two ways of putting on the hats are considered different if the hats on at least one head of one of the plush toys are of different colors.

<ASSISTANT>
Pola can put the hats on her plush toys in **65 different ways** so that each head has exactly one hat.

<WRITTEN AND EXECUTED CODE>
from math import factorial

# Total heads
total_heads = 5

# Number of hats of each color
white_hats = 4
green_hats = 2
red_hats = 1

# Since each head must have exactly one hat, we are distributing 5 hats on 5 heads:
# - 4 white hats (identical)
# - 2 green hats (identical)
# - 1 red hat (unique)

# We will count the number of distinct permutations considering identical hats.

# Possible distributions:
# 1. Use 4 white + 1 red (can't use green here, since we have 2 green hats).
#    Arrangement: 4W, 1R
ways_4W_1R = factorial(5) // (factorial(4) * factorial(1))

# 2. Use 3 white + 2 green
ways_3W_2G = factorial(5) // (factorial(3) * factorial(2))

# 3. Use 3 white + 1 green + 1 red
ways_3W_1G_1R = factorial(5) // (factorial(3) * factorial(1) * factorial(1))

# 4. Use 2 white + 2 green + 1 red
ways_2W_2G_1R = factorial(5) // (factorial(2) * factorial(2) * factorial(1))

# Add all possibilities
total_ways = ways_4W_1R + ways_3W_2G + ways_3W_1G_1R + ways_2W_2G_1R

total_ways
