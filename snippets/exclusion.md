		 ---
 title: Exclusion
 tags: array,beginner
 ---
  Compare two arrays and remove duplicates from first one
 
 - Use `Array.prototype.filter()` to pass the test implemented by the provided function.
 - Use `Array.prototype.includes()` to determine whether an array includes a certain value among its entries.
 
  ```js

let exclusion = (a,b) => {
 return a = a.filter((val) => !b.includes(val));
} 
 ```

 ```js
let first = ['10:00','11:00','string',2]
let second = [2,4, 'string', '10:00']

exclusion(first, second); // [ '11:00' ]
 ```