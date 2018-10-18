# Exercise 2.3.5:

The relational-algebra operation R(A,B) ⊲⊳ B<C S(C,D) produces all tuples (a,b,c,d) 
such that tuple (a,b) is in relation R, tuple (c,d) is in S,
and b < c. Give a map-reduce implementation of this operation, assuming R and S are sets.
# solution

## Map Function
For each tuple (a,b) of R, the key-value is (R, (a,b)). For each tuple (c,d) of S, the key-value is (S,(c,d)) 
