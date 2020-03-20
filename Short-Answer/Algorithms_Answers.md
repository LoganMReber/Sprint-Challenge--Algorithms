#### Please add your answers to the **_Analysis of Algorithms_** exercises here.

## Exercise I

a) The big O time is O(n). This is because that loop's condition is n^3 and n^2 is the increment.

b) The big O time is O(nlog(n)). This is because loop 1's condition is 0 to n-1 and the increment is 1.
This gives the loop n runtime. The second loop's is 1 to n-1 where the increment is j\*=2. This is log(n)
runtime. Nested loops multiply together for nlog(n).

c) The big O time is O(n). This is because the function uses recursion until n is 0 at a rate of -1 per recursion.

## Exercise II

Alg:

```py
findFloor(floors,top,bottom,prev)
    if top - bottom < 2
        return top
    floor = top / bottom
    if egg survives
        if prev-1 == floor
            return floor
        else
            return findFloor(floors,top,floor,floor)
    else
        if prev+1 == floor
            return prev
        else
            return findFloor(floors,floor,bottom,floor)
```

Time/Eggs Dropped: 0(log(n))

Reasoning: Floors are sorted so using a binary search allows a max of about log(n) attempts
