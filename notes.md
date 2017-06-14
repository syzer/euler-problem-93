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
1 
- [ ] upper bound not set, so maybe :
    - calc non expressible number
    - try to find next one
    - fnd longest distance between those
    - upper bound is 9
    - recursive solution? greedy to killoff branches with non expresssible solution?
