## Slice and Splice

You are given two arrays and an index.

Use the array methods `slice` and `splice` to copy each element of the first array into the second array, in order.

Begin inserting elements at index `n` of the second array.

Return the resulting array. The input arrays should remain the same after the function runs.

#### Before

```javascript
function frankenSplice(arr1, arr2, n) {
  return arr2;
}

frankenSplice([1, 2, 3], [4, 5, 6], 1);

```

#### Answers

```javascript
function frankenSplice(arr1, arr2, n) {

  let arr3 = arr2.slice(0, arr2.length);

  for (let i = arr1.length - 1; i >= 0; i--) {
    arr3.splice(n, 0, arr1[i]);
  }

  return arr3;
}

frankenSplice([1, 2, 3], [4, 5, 6], 1);

```