---
layout: essay
type: essay
title: Coding Standards
# All dates must be YYYY-MM-DD format!
date: 2019-02-07
labels:
  - ESLint
  - JavaScript
  - IntelliJ
---

## ESLint
At the moment, I find ESLint to be a bit tedious and distracting but still very useful. One aspect that is confusing is when I declare an empty array with `let`, I plan on changing the array by pushing values to the array. Since I know the array will change I use `let`, but ESLint tells me that the variable for the array is never reassigned, and `const` should be used instead. Here is an example:
```javascript
function fib() {
  let result = [];
  let current = 0;
  let next = 1;
  let temp;
  for (let i = 0; i < 100; i++) {
    result.push(current);
    temp = current;
    current = next;
    next = current + temp;
  }
  return result;
}
```
In this code snippet, ESLint will give me an error that says "ESLint: 'result' is never reassigned. Use 'const' instead. (prefer-const)."

The aspect I find tedious is just the space formatting. 

Sometimes it can be a bit distracting while I am writing a function in the beginning when I only declare the variables but don't do anything to them yet. It says "ESLint: variable is defined but never used (no-unused-vars)". For example, if I comment out the whole for-loop, ESLint will show an error with the variables `current`, 


## IntelliJ



