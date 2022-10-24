1. Construct a function intersection that compares input arrays and returns a new array with elements found in all of the inputs. You can only use reduce method to do this.

```js
function intersection(...arrays) {
  //find the smallest array
  let count = Infinity;
  let subArr = [];
  for (let i = 0; i < arrays.length; i++) {
    if (count > arrays[i].length) {
      count = arrays[i].length;
      subArr = arrays[i];
    }
  }

  //iterate over its elements
  let ignore = [];
  for (let j = 0; j < subArr.length; j++) {
    for (let k = 0; k < arrays.length; k++) {
      if (!arrays[k].includes(subArr[j])) {
        ignore.push(subArr[j]);
      }
    }
  }

  let resArr = [];
  for (let item of subArr) {
    if (!ignore.includes(item)) {
      resArr.push(item);
    }
  }

  return resArr;
}



// Test
console.log(
  intersection(
    [5, 10, 15, 20],
    [15, 88, 1, 5, 7],
    [1, 10, 15, 5, 20]
  )
); // should log: [5, 15]
```

2. Construct a function `union` that compares input arrays and returns a new array that contains all elements. If there are duplicate elements, only add it once to the new array. Preserve the order of the elements starting from the first element of the first input array. You can only use reduce method to do this.

```js
function union(...arrays) {
  //find the largest array
  let count = 0;
  let subArr = [];
  for (let i = 0; i < arrays.length; i++) {
    if (count < arrays[i].length) {
      count = arrays[i].length;
      subArr = arrays[i];
    }
  }

let resArr = [];

for ( let i = 0; i < arrays.length; i++ ) {
   for (let item of arrays[i]) {
    if(!resArr.includes(item)) {
        resArr.push(item);
      }
   }
}
  
return resArr;
  
  // iterate over the largest array

  // include every non repeating item
}


// Test
console.log(
  union([5, 10, 15], [15, 88, 1, 5, 7], [100, 15, 10, 1, 5])
);
// should log: [5, 10, 15, 88, 1, 7, 100]
```
