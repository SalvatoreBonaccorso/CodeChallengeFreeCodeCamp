## Falsy Bouncer

Remove all falsy values from an array.
Falsy values in JavaScript are `false, null, 0, "", undefined, and NaN`.
Hint: Try converting each value to a Boolean.

#### Before

```javascript
function bouncer(arr) {
  return arr;
}

bouncer([7, "ate", "", false, 9]);
```

#### Answers

```javascript
function bouncer(arr) {

  return arr.filter(Boolean);
  
}

bouncer([7, "ate", "", false, 9]);

```