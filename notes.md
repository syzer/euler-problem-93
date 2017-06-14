```bash
parse to AST => flatMap
parse AST =? flatmap
```
can it 
greedy?

1 = (1) + 2 - 3 + 4
2 = (1 + 2) * (3 - 4)

rb tree ?
.. not balance.. maybe reduce and minimize with memoization ?

1 2 3 4

     3
    / \
   2  4
  / \     
 1
           + 
         /   \
        4     2
       / \   / \
      3  -  1  -
2 = (4 - 3) + 2 - 1

- [ ] debug on 29 => cannot be obtained
- [ ] is it LCS/ GCD / divisor problem again?
2^6 permutation => calc => Map => length
64 permutation.. ~31 legal
576 cases


1+2+3+4
1+2+3-4
1+2-3-4
-------
1-2-3-4
- [ ] upper bound not set, so maybe :
    - calc non expressible number
    - try to find next one
    - fnd longest distance between those
    - upper bound is 9
    - recursive solution? greedy to kill off branches with non expresssible solution?
- max sum number calc 6*7*8*9 = 3024
next representable number is
so we can skip numbers bigger than 510
so better to count from top
510 = 6+7*8*9
498 = 7*8*9-6
425 = 6*8*9-7
345 = 6*7*8+9 
114 = 6*7+8*9 next representable number

- brute force:
all posible permutations ot 4 numbers
all posible permutations of operations