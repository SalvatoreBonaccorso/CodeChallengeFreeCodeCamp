## Repeat a String Repeat a String

Repeat a given string `str` (first argument) for `num` times (second argument). Return an empty string if `num` is not a positive number.

#### Before

```javascript
function repeatStringNumTimes(str, num) {
  return str;
}

repeatStringNumTimes("abc", 3);

```

#### Answers

```javascript
function repeatStringNumTimes(str, num) {

  let sum = "";

  if (num <= 0) {
    return sum;
  }

  for (let i = 0; i < num; i++) {
    sum += str;
  }
  return sum;
}

repeatStringNumTimes("abc", 3);

```