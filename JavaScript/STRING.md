## extract a substring from a string

We can use substring or slice
```js
let str = "Hello, world!";
let result = str.substring(7, 12); // This method returns a part of the string between two specified indices.
console.log(result); // Output: "world"

let subStr = str.slice(7, 12);  // Extracts characters from index 7 to 12
console.log(subStr);  // Output: "world"

let subStrFromEnd = str.slice(-6, -1);  // Extracts the last 6 characters
console.log(subStrFromEnd);  // Output: "world"

let subStrTillEnd = str.slice(2);  // if we omit second param it return till the end of the string
console.log(subStrTillEnd);  // Output: "llo, world!"
console.log(str.substring(2));  // Output: "llo, world!"

```
