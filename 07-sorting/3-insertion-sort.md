# Insertion Sort
Builds up the sort by gradually creating a larger left half which is always sorted. 
We take one element and insert it in the right place in the sorted part. One advantage over bubble and selection sort is that it is good when the data is nearly sorted. 

## Complexity
1. Time
* Best: O(n)
* Avg: O(n<sup>2</sup>)
* Worst: O(n<sup>2</sup>)


2. Space
* All: O(1)

## Implementation
```javascript
function insertionSort(array) {
    for (let i = 0; i < array.length - 1; i++)
        for (let j = i + 1; j > 0; j--)
            if (array[j] < array[j - 1])[array[j - 1], array[j]] = [array[j], array[j - 1]];
            else break;
}
```
