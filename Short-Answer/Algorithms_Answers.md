#### Please add your answers to the **_Analysis of Algorithms_** exercises here.

## Exercise I

a) O(n) (Linear) time complexity since operations grow with the size of the input. See Examples Below:

```
n=2

a=0
while (a < 8):
    a = 0 + 4

while (a < 4):
    a = 4 + 4;

a = 0
n = 3
while (a < 27):
    a = 0 + 9

while (9 < 27):
    a = 9 + 9

while (18 < 27):
    a = 18 + 9
```

b) O(n log n) - 'Linearithmic' Time

First loop is O(n) since operations grow with the size of n.
Second loop requires 1 less operation than prior loop since it's multiplied by a constant amount (O(Logn))

c) O(n) - Linear time since the amount of recursive calls completed depends upon the size of the input.

## Exercise II

Runtime complexity -> O(log n)

We want to calculate the midpoint of the building and drop the egg from that point. We also store the top level of the building and the bottom level of the building. If the egg breaks at the midpoint, we move the top down to the midpoint - 1, recalculate the midpoint, and drop the egg again. If the egg doesn't break, move the bottom point to the midpoint plus one, recalculate the midpoint and drop the egg again. When the two points overlap, we've found the point at which the egg can be dropped safely.
