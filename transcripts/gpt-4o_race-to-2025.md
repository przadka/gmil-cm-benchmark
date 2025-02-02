<USER>
### 4. Race to 2025!

```
   G N A J
+     N A
-----------
   2 0 2 5
```

In this coded addition, different letters represent different digits, and the same digit is always represented by the same letter. Additionally, none of the multi-digit numbers start with zero.

**What is the value of NA?**

<ASSISTANT>
The value of **NA** is **93**.

<WRITTEN AND EXECUTED CODE>
# Brute-force approach to find the solution

from itertools import permutations

# Possible digits
digits = range(10)

# Trying all permutations for the letters G, N, A, J
for perm in permutations(digits, 5):  # G, N, A, J, and the extra 2 for carry
    G, N, A, J, extra = perm
    
    # Constraints: None of the multi-digit numbers start with zero
    if G == 0 or N == 0:
        continue
    
    # Form the numbers
    GNAJ = G * 1000 + N * 100 + A * 10 + J
    NA = N * 10 + A
    total = GNAJ + NA

    # Check if the sum is 2025
    if total == 2025:
        result = NA
        break

result
