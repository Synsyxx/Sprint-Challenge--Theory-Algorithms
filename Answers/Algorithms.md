## Analysis of Algorithms

### Exercise I.
*Give an analysis of the running time with respect to the input size n of each of the following program fragments below:*

___

1. O(n)
2. O(log n)
3. O(n*2
4. O(n log n)
5. O(n^4)
6. O(n)
7. O(n)


### Exercise II.
1. const max = (values) => {<br/>
    let high = 0;<br/>
    for (let i = 0; i < values.length; i++) {<br/>
        if (values[i] < values[i + 1]) {<br/>
            high = values[i + 1];<br/>
        }<br/>
    }<br/>
    return high;<br/>
};

2.  Binary Search Tree:
    Start from floor ` f = n/2 `<br/>
    If the egg breaks, move down to ` f = f/2 ` <br/>
    Otherwise, move up to ` f = f + (n - f)/2 `<br/>

    Stop searching when the egg doesn't break at ` f `, <br/>
    and the egg breaks at ` f + 1`.
    This gives the value of f. 

### Exercise III.

1. Time complexity would be O(n^2) because it has to iterate through the entire array

2. Time complexity would be O(n log n) because the array is split in 2 almost equal sizes at each step, so there will be (log n) number of steps, and each step is in a
linear O(n) time complexity.