## Finders Keepers
Create a function that looks through an array (first argument) and returns the first element in the array that passes a truth test (second argument). If no element passes the test, return undefined.


#### Before
```javascript
function findElement(arr, func) {
  let num = 0;
  return num;
}

findElement([1, 2, 3, 4], num => num % 2 === 0);
```

#### Answers

```javascript
function findElement(arr, func) {

  for(let i=0; i<arr.length; i++){
    let result = func(arr[i]);
    if (result == true ){
        return arr[i];
    }
  }
  return undefined;

}

findElement([1, 3, 5, 8, 9, 10], num => num % 2 === 0);

```