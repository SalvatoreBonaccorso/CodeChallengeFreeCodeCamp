## Chunky Monkey

Write a function that splits an array (first argument) into groups the length of `size` (second argument) and returns them as a two-dimensional array.

#### Before

```javascript
function chunkArrayInGroups(arr, size) {
  return arr;
}

chunkArrayInGroups(["a", "b", "c", "d"], 2);
```

#### Answers

```javascript
function chunkArrayInGroups(arr, size) {

let result = [];
let count=0;

  while(count < arr.length) {
    result.push(arr.slice(count, count += size));
  }
  
  return result;
}

chunkArrayInGroups(["a", "b", "c", "d"], 2);

```