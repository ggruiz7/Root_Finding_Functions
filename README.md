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

## Fixed-Point Iteration
The fixed point iteration method works by repeatedly applying the function f to an initial guess
x0, generating a sequence of approximations x1, x2, x3, …, until convergence to a fixed point is
achieved within a desired tolerance. The algorithm works as follows:
Choose an initial guess x0. Compute the next approximation x1 by applying the function f to x0,
i.e., x1 = f(x0). Check if the absolute value of the difference between x1 and x0 is less than a
desired tolerance. If it is, return x1 as the fixed point. Otherwise, set x0 = x1 and repeat step
2. The method is guaranteed to converge to a fixed point if f is a contraction mapping, which
means that it satisfies a Lipschitz condition with constant less than 1. In practice, the method may
converge slowly or not at all if f is not a contraction mapping or if the initial guess is far from the
fixed point.
