## Reverse a String

Reverse the provided string.
You may need to turn the string into an array before you can reverse it.
Your result must be a string.

#### Before

```javascript
function reverseString(str) {
  return str;
}

reverseString("hello");
```

#### Answers

```javascript
function reverseString(str) {

  let result = [];

  str = str.split("");

  for (let i = str.length - 1; i >= 0; i--) {
    result.push(str[i]);
  }

  result = result.join("");

  return result;
}

reverseString("hello");

```