## Title Case a Sentence

Return the provided string with the first letter of each word capitalized. Make sure the rest of the word is in lower case.
For the purpose of this exercise, you should also capitalize connecting words like "the" and "of".

#### Before

```javascript
function titleCase(str) {
  return str;
}

titleCase("I'm a little tea pot");
```

#### Answers

```javascript
function titleCase(str) {
  
  let string = str.toLowerCase();

  let strArray = string.split(" ");
  let emptyArray = [];

  for (let i = 0; i < strArray.length; i++) {
    emptyArray[i] = strArray[i].charAt(0).toUpperCase()+ strArray[i].slice(1)
  }
  return emptyArray.join(" ");
}

titleCase("I'm a little tea pot");

```