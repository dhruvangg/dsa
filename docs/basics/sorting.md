---
sidebar_position: 1
---

# Sorting

A Sorting Algorithm is used to rearrange a given array or list of elements according to a comparison operator on the elements. The comparison operator is used to decide the new order of elements in the respective data structure.

## Bubble Sort

**Bubble sort** algorithm is an algorithm that sorts an array by comparing two neighboring elements and swapping them if they are not in the desired order. Here order can be anything like increasing or decreasing.

Refer: https://www.w3schools.com/dsa/dsa_algo_bubblesort.php

```js title="bubbleSort.js"
const bubbleSort = (arr) => {
    for (let j = 0; j < arr.length; j++) {
        let swapped;
        for (let i = 0; i < arr.length; i++) {
            if (arr[i] > arr[i + 1]) {
                var temp = arr[i];
                arr[i] = arr[i + 1]
                arr[i + 1] = temp
                swapped = true;
            }
        }
        if(!swapped)
            break;
    }
    return arr;
}
```