# JavaScript Promises

## Creating a Promise

| Syntax | Description | Example | Output |
|---|---|---|---|
| `new Promise()` | Creates a new promise | `new Promise((resolve, reject) => resolve("Done"))` | `Promise { "Done" }` |



## Static Methods

| Method | Description | Example | Output |
|---|---|---|---|
| `Promise.resolve()` | Returns a resolved promise | `Promise.resolve(10)` | `Promise { 10 }` |
| `Promise.reject()` | Returns a rejected promise | `Promise.reject("Error")` | `Promise { <rejected>: "Error" }` |
| `Promise.all()` | Waits for all promises to resolve (fails if one fails) | `Promise.all([p1, p2])` | `Array of results` |
| `Promise.allSettled()` | Waits for all promises (success or fail) | `Promise.allSettled([p1, p2])` | `Array of status objects` |
| `Promise.race()` | Returns first settled promise | `Promise.race([p1, p2])` | `First result` |
| `Promise.any()` | Returns first fulfilled promise | `Promise.any([p1, p2])` | `First success value` |



## Instance Methods

| Method | Description | Example | Output |
|---|---|---|---|
| `.then()` | Handles successful result | `p.then(res => console.log(res))` | Returns new Promise |
| `.catch()` | Handles errors | `p.catch(err => console.log(err))` | Returns new Promise |
| `.finally()` | Runs after completion (success or fail) | `p.finally(() => console.log("Done"))` | Returns new Promise |



## Example Usage

```js
const myPromise = new Promise((resolve, reject) => {
  const success = true;

  if (success) {
    resolve("Operation successful");
  } else {
    reject("Operation failed");
  }
});

myPromise
  .then(result => console.log(result))
  .catch(error => console.log(error))
  .finally(() => console.log("Finished"));
