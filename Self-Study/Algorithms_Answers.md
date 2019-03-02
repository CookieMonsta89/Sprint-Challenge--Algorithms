```
a)  a = 0
    while (a < n * n * n):
      # 0(n) 
      a = a + n * n
```
1. I'd say that htis is 0(n) because if n is increased then the amount of loops that have to run will be increased

```
b)  sum = 0

    for i in range(n): 0(n)
      i += 1           
      for j in range(i + 1, n):  O(n)
        j += 1
        for k in range(j + 1, n): 0(n)
          k += 1
          for l in range(k + 1, 10 + k): 0(c)
            l += 1
            sum += 1
```

2. O(n^3).  
 O(n*n*n*c)
 O(n*n*n)
 O(n^3)
```
c)  def bunnyEars(bunnies):  #went over this with Luisan in class :)
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)
```
3. This will be 0(n) as the number increases the function will call itself. 

#### Exercise II

```Suppose that you have an _n_-story building and plenty of eggs. Suppose also
that an egg gets broken if it is thrown off floor _f_ or higher, and doesn't get
broken if dropped off a floor less than floor _f_. Devise a strategy to
determine the value of _f_ such that the number of dropped eggs is minimized.

Write out your proposed algorithm in plain English or pseudocode and give the
runtime complexity of your solution.```

-So I have a building that is n stories tall.
-when egg is dropped from f floor or higher, it will break.
-when egg is dropped from any floor less than f, it will not break.
 So the floors are already sorted. I'd find the middle floor of the stories and I would drop my egg from there. If the egg does not break, I would now make that floor my bottom floor and I'd find the middle floor again. If the egg broke initially, that would be the top floor and I'd find the middle and repeat.  I'd continue this method until I fount f floor. We learned about this method early in Algorithms and it is called Binary search. I'm certain binary search has a time complexity of O(log n). Increases the number of operations it performs as a logarithmic function of the input size (n)



