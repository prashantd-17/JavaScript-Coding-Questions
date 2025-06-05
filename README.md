# JavaScript Coding Questions

### Table of Contents

<!-- TOC_START -->
| No. | Questions |
| --- | --------- |
| 1 | [Rotate array at given index](#1-rotate-array-at-given-index) |
---

## 1. Rotate array at given index

### Question:
Rotate the given array at a given index without using in-built functions.

```js
// Input: [1,2,3,4,5,6], Index: 3
// Output: [4,5,6,1,2,3]

// Method 1
const input1 = [1,2,3,4,5,6];
const index = 3;
const arr1 = [];
const arr2 = [];
for (let i = 0; i < input1.length; i++) {
  if (index <= i) {
    arr1.push(input1[i]);
  } else {
    arr2.push(input1[i]);
  }
}
const numsnew = [...arr1, ...arr2];
console.log(numsnew);

