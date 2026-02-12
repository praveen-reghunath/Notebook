
### debouncing

Debouncing is a way of delaying the execution of a function until a certain amount of time has passed since the last time it was called. This can be useful for scenarios where we want to avoid unnecessary or repeated function calls that might be expensive or time-consuming.

eg: Search box: When you type something in a search box, it doesn’t show suggestions on every keystroke, but waits until you stop typing for a while.

```
const debounce = (mainFunction, delay) => {
    // Declare a variable called 'timer' to store the timer ID
    let timer;
  
    // Return an anonymous function that takes in any number of arguments
    return function (...args) {
      // Clear the previous timer to prevent the execution of 'mainFunction'
      clearTimeout(timer);
  
      // Set a new timer that will execute 'mainFunction' after the specified delay
      timer = setTimeout(() => {
        mainFunction(...args);
      }, delay);
    };
  };
```

Now use the function some where like bellow. 

```
// Define a function called 'searchData' that logs a message to the console
function search() {
  console.log("searchData executed");
}

// Create a new debounced version of the 'searchData' function with a delay of 3000 milliseconds (3 seconds)
const debouncedSearch = debounce(search, 3000);

// Call the debounced version of 'search' on every key press.
debouncedSearch();
```
