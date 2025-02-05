## extract a substring from a string

We can use substring or slice
```
let str = "Hello, world!";
let result = str.substring(7, 12); // This method returns a part of the string between two specified indices.
console.log(result); // Output: "Hello"

let subStr = str.slice(7, 12);  // Extracts characters from index 7 to 12
console.log(subStr);  // Output: "World"

let subStrFromEnd = str.slice(-6, -1);  // Extracts the last 6 characters
console.log(subStrFromEnd);  //
```
