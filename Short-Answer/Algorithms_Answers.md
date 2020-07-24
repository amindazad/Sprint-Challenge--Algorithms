#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

```python
# This is O(1)
a)  a = 0
# This loop will run O(n)times
    while (a < n * n * n):
    # a is incremented (n**2) each time
    # multiplication, addition and assignment is O(1)
      a = a + n * n
      # Total time complexity = O(1+n+1) --> O(n)
```


```python
# This is O(1)
b)  sum = 0
# The outer loop runs in O(n) * the complexity of the inner loop
    for i in range(n):
    # This is O(1)
      j = 1
      # j doubles every iterations so this loop will run in O(log n)
      while j < n:
        # This is O(1)
        j *= 2
        # This is O(1)
        sum += 1
        #Total time complexity = O(1) + O(n) * (O(log n) + O(1+1))
        #                       = O(1) + O(n) * O(log n)
        #                       = O(n log n)
```

```python
c)  def bunnyEars(bunnies):
    # This is O(1)
      if bunnies == 0:
        return 0
    # The state of bunnies decreases by 1 each recursion
    # So bunnies recurse n times 
      return 2 + bunnyEars(bunnies-1)
    # Total time complexity = O(1) + O(n) = O(n)
'''
    
## Exercise II


