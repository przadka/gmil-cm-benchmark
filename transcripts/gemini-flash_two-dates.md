<USER>
### 1. Two Dates

Mateusz has 12 cards with digits:

`0 0 1 1 2 2 3 3 4 4 5 5`

and he arranges them to form dates. The first date of 2025 that he can create using two cards to form the day number, two other cards to form the month number, and four other cards to form the year number will be January 13:

`1 3 0 1 2 0 2 5`

**What will be the last date in 2025 that Mateusz can create using eight of these twelve cards?**

<ASSISTANT>
Here's how to figure out the last possible date Mateusz can make in 2025:

1. **Year:** The year is fixed as 2025.

2. **Month:** We want the *last* possible date, so we should aim for the latest possible month.  The available digits allow us to make "12" (December).

3. **Day:** Now we need the latest possible *day* within December.  We have the digits 0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5.  We've used 2 and 5 for the year, 1 and 2 for the month.  This leaves us with 0, 0, 1, 1, 3, 3, 4, 4. The largest day we can form is 31.

Therefore, the last possible date is December 31, 2025, represented as `3 1 1 2 2 0 2 5`.
