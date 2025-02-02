<USER>
### 8. Hats

Pola has a pair of plush monsters: a three-headed Cerberus and a two-headed Dragon. She really enjoys playing with these plush toys by putting hats on their heads. Pola has four identical white hats, two identical green hats, and one red hat. It is known that each of these hats can be placed on any head of Cerberus or the Dragon.

**In how many different ways can Pola put the hats on her plush toys so that each head has exactly one hat?**  
Two ways of putting on the hats are considered different if the hats on at least one head of one of the plush toys are of different colors.

<ASSISTANT>
Here's how to solve this combinatorics problem:

**1. Distribute the hats:**

* **Cerberus (3 heads):** We need to choose 3 hats out of the 7 total hats.  Since some hats are identical, we'll consider the cases:
    * 3 white hats:  There's only 1 way to do this (all white hats).
    * 2 white hats, 1 green hat:  There are 2 ways to choose which green hat goes on (2 green hats).
    * 2 white hats, 1 red hat: There's only 1 way to do this (1 red hat).
    * 1 white hat, 2 green hats: There's only 1 way to do this (2 green hats).
    * 1 white hat, 1 green hat, 1 red hat: There are 2 * 1 = 2 ways to do this (2 green hats).
* **Dragon (2 heads):**  We need to choose 2 hats out of the remaining 4 hats.
    * 2 white hats: 1 way.
    * 2 green hats: 1 way.
    * 1 white hat, 1 green hat: 1 way.
    * 1 white hat, 1 red hat: 1 way.
    * 1 green hat, 1 red hat: 1 way.

**2. Combine the possibilities:**

Now, we multiply the number of ways to dress Cerberus with the number of ways to dress the Dragon for each possible distribution of hats.

* **Case 1: Cerberus (3W), Dragon (2W):** 1 way * 1 way = 1 way
* **Case 2: Cerberus (2W, 1G), Dragon (2W):** 2 ways * 1 way = 2 ways
* **Case 3: Cerberus (2W, 1R), Dragon (2W):** 1 way * 1 way = 1 way
* **Case 4: Cerberus (1W, 2G), Dragon (2W):** 1 way * 1 way = 1 way
* **Case 5: Cerberus (1W, 1G, 1R), Dragon (2W):** 2 ways * 1 way = 2 ways
* **Case 6: Cerberus (3W), Dragon (2G):** 1 way * 1 way = 1 way
* **Case 7: Cerberus (2W, 1G), Dragon (2G):** 2 ways * 1 way = 2 ways
* **Case 8: Cerberus (2W, 1R), Dragon (2G):** 1 way * 1 way = 1 way
* **Case 9: Cerberus (1W, 2G), Dragon (2G):** 1 way * 1 way = 1 way
* **Case 10: Cerberus (1W, 1G, 1R), Dragon (2G):** 2 ways * 1 way = 2 ways
* **Case 11: Cerberus (3W), Dragon (1W, 1G):** 1 way * 1 way = 1 way
* **Case 12: Cerberus (2W, 1G), Dragon (1W, 1G):** 2 ways * 1 way = 2 ways
* **Case 13: Cerberus (2W, 1R), Dragon (1W, 1G):** 1 way * 1 way = 1 way
* **Case 14: Cerberus (1W, 2G), Dragon (1W, 1G):** 1 way * 1 way = 1 way
* **Case 15: Cerberus (1W, 1G, 1R), Dragon (1W, 1G):** 2 ways * 1 way = 2 ways
* **Case 16: Cerberus (3W), Dragon (1W, 1R):** 1 way * 1 way = 1 way
* **Case 17: Cerberus (2W, 1G), Dragon (1W, 1R):** 2 ways * 1 way = 2 ways
* **Case 18: Cerberus (2W, 1R), Dragon (1W, 1R):** 1 way * 1 way = 1 way
* **Case 19: Cerberus (1W, 2G), Dragon (1W, 1R):** 1 way * 1 way = 1 way
* **Case 20: Cerberus (1W, 1G, 1R), Dragon (1W, 1R):** 2 ways * 1 way = 2 ways
* **Case 21: Cerberus (3W), Dragon (1G, 1R):** 1 way * 1 way = 1 way
* **Case 22: Cerberus (2W, 1G), Dragon (1G, 1R):** 2 ways * 1 way = 2 ways
* **Case 23: Cerberus (2W, 1R), Dragon (1G, 1R):** 1 way * 1 way = 1 way
* **Case 24: Cerberus (1W, 2G), Dragon (1G, 1R):** 1 way * 1 way = 1 way
* **Case 25: Cerberus (1W, 1G, 1R), Dragon (1G, 1R):** 2 ways * 1 way = 2 ways

Adding all these possibilities: 1 + 2 + 1 + 1 + 2 + 1 + 2 + 1 + 1 + 2 + 1 + 2 + 1 + 1 + 2 + 1 + 2 + 1 + 1 + 2 + 1 + 2 + 1 + 1 + 2 = 30

**Therefore, there are 30 different ways Pola can put the hats on her plush toys.**
