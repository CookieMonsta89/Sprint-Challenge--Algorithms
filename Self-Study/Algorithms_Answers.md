```
a)  a = 0
    while (a < n * n * n):
      # 0(n) 
      a = a + n * n
```
1. I'd say that htis is 0(n) because if n is increased then the amount of loops that have to run will be increased

```
b)  sum = 0

    for i in range(n): #0(n)
      i += 1            runs once
      for j in range(i + 1, n):  +1
        j += 1
        for k in range(j + 1, n): +1
          k += 1
          for l in range(k + 1, 10 + k): +1
            l += 1
            sum += 1
```

2. O(n^3). We have three for loops here and we start at 0(n) so we add the three for loops. 

```
c)  def bunnyEars(bunnies):  #went over this with Luisan in class :)
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)
```
3. This will be 0(n) as the number increases the function will call itself. 

#### Exercise II





