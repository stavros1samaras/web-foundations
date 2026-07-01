# JavaScript Array

## Static Methods

| Syntax | Description | Example | Output |
|---|---|---|---|
| `Array.isArray()` | Checks if a value is an array | `Array.isArray([1,2,3])` | `true` |
| `Array.from()` | Creates a new array from iterable or array-like object | `Array.from("abc")` | `["a","b","c"]` |
| `Array.of()` | Creates a new array from arguments | `Array.of(1,2,3)` | `[1,2,3]` |
| `Array.concat()` | Merges arrays (static call rarely used, instance preferred) | `[].concat([1,2],[3,4])` | `[1,2,3,4]` |

## Instance Methods (Prototype)

| Syntax | Description | Example | Output |
|---|---|---|---|
| `.push()` | Adds elements to the end | `[1,2].push(3)` | `3` (new length) |
| `.pop()` | Removes last element | `[1,2,3].pop()` | `3` |
| `.shift()` | Removes first element | `[1,2,3].shift()` | `1` |
| `.unshift()` | Adds elements to the start | `[2,3].unshift(1)` | `3` (new length) |
| `.concat()` | Merges arrays | `[1,2].concat([3,4])` | `[1,2,3,4]` |
| `.slice()` | Extracts part of array | `[1,2,3,4].slice(1,3)` | `[2,3]` |
| `.splice()` | Adds/removes elements | `[1,2,3,4].splice(1,2,"a","b")` | `[2,3]` (removed) |
| `.indexOf()` | Returns first index of element | `[1,2,3,2].indexOf(2)` | `1` |
| `.lastIndexOf()` | Returns last index of element | `[1,2,3,2].lastIndexOf(2)` | `3` |
| `.includes()` | Checks if element exists | `[1,2,3].includes(2)` | `true` |
| `.forEach()` | Iterates over elements | `[1,2,3].forEach(x => console.log(x))` | `1 2 3` |
| `.map()` | Creates new array with function applied | `[1,2,3].map(x => x*2)` | `[2,4,6]` |
| `.filter()` | Creates new array with elements passing test | `[1,2,3].filter(x => x>1)` | `[2,3]` |
| `.reduce()` | Reduces array to single value | `[1,2,3].reduce((a,b)=>a+b,0)` | `6` |
| `.reduceRight()` | Reduces from right to left | `[1,2,3].reduceRight((a,b)=>a-b,0)` | `-6` |
| `.sort()` | Sorts elements | `[3,1,2].sort()` | `[1,2,3]` |
| `.reverse()` | Reverses array | `[1,2,3].reverse()` | `[3,2,1]` |
| `.join()` | Joins elements into string | `[1,2,3].join("-")` | `"1-2-3"` |
| `.find()` | Returns first element passing test | `[1,2,3].find(x => x>1)` | `2` |
| `.findIndex()` | Returns index of first element passing test | `[1,2,3].findIndex(x => x>1)` | `1` |
| `.every()` | Checks if all elements pass test | `[1,2,3].every(x => x>0)` | `true` |
| `.some()` | Checks if at least one element passes test | `[1,2,3].some(x => x>2)` | `true` |
| `.flat()` | Flattens nested arrays | `[1,[2,3],[4]].flat()` | `[1,2,3,4]` |
| `.flatMap()` | Maps then flattens array | `[1,2,3].flatMap(x => [x, x*2])` | `[1,2,2,4,3,6]` |
| `.fill()` | Fills array with value | `[1,2,3].fill(0)` | `[0,0,0]` |
| `.copyWithin()` | Copies part of array within itself | `[1,2,3,4].copyWithin(0,2)` | `[3,4,3,4]` |

## Instance Properties

| Property | Description | Example | Output |
|---|---|---|---|
| `.length` | Number of elements in the array | `[1,2,3].length` | `3` |
