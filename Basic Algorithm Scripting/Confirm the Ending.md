## Confirm the Ending

Check if a string (first argument, `str`) ends with the given target string (second argument, `target`).

This challenge can be solved with the `.endsWith()` method, which was introduced in ES2015. But for the purpose of this challenge, we would like you to use one of the JavaScript substring methods instead.

#### Before
```javascript
function confirmEnding(str, target) {
  return str;
}

confirmEnding("Bastian", "n");

```

#### Answers

```javascript
function confirmEnding(str, target) {

  // step 1 convert to array target and str
  let targetArray = target.split("");
  let strArray = str.split("");

  // step 2 create an empty array
  let finalWords = [];

  // step 3 loop for 
  for (let i = strArray.length - 1; i > (strArray.length - 1) - targetArray.length; i--) {
    finalWords.unshift(strArray[i]);
  }

  // step 4 finalWords convert to string
  let x = finalWords.join("");

  // step 5 condition
    return x == target;

}

console.log(confirmEnding("Open sesame", "pen"));


```