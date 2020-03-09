## Find the Longest Word in a String

Return the length of the longest word in the provided sentence.

Your response should be a number.

#### Before

```javascript
function findLongestWordLength(str) {
  return str.length;
}

findLongestWordLength("The quick brown fox jumped over the lazy dog");
```

#### Answers

```javascript
function findLongestWordLength(str) {

  let arr = str.split(' ');
  let max = 0;

  for (let i = 0; i < arr.length; i++) {
    let valStr = arr[i].length;

    if (valStr > max) {
      max = valStr;
    }
  }
  return max;
}

findLongestWordLength("The quick brown fox jumped over the lazy dog");

```