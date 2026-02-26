
## While writting sort functions; write the return value in the order we define params to get ASC order

```js
[-1, 0, 1, 2, -1, -4].sort((a,b)=> a-b); // will sort in ASC order
[-1, 0, 1, 2, -1, -4].sort((a,b)=> b-a); // for DESC order 

```
