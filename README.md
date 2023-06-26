## The Bisection Method
Given an interval [a, b] where the function changes sign, the method repeatedly bisects the interval
and selects the subinterval in which the function changes sign, until the root is located within a
desired tolerance. The algorithm works as follows:
Begin with an interval [a, b] where the function changes sign. Compute the midpoint c = (a +
b)/2. Evaluate the function at c. If the function at c is close enough to zero (i.e., within the desired
tolerance), then return c as the root. Otherwise, determine which subinterval [a, c] or [c, b] has a
sign change, and repeat the algorithm on that subinterval. The bisection method is guaranteed to
converge to a root of the function as long as the function is continuous and changes sign within the
interval [a, b]. However, it can be slow to converge for functions that are very flat near the root,
or for intervals that are very wide.
