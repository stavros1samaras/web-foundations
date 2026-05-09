| Expression   | `typeof`  | `instanceof`  | Prototype Chain |
|--------------|------------------|--------------------|------------------|
| `42` | `"number"` | — | No prototype chain |
| `"text"` | `"string"` | — | No prototype chain |
| `true` | `"boolean"` | — | No prototype chain |
| `Symbol("id")` | `"symbol"` | — | No prototype chain |
| `42n` | `"bigint"` | — | No prototype chain |
| `undefined` | `"undefined"` | — | No prototype chain |
| `null` | ⚠️ `"object"` | — | No prototype chain |
| `[]` | `"object"` | `instanceof Array` | `Array.prototype → Object.prototype → null` |
| `Array` | `"function"` | `instanceof Function` | `Function.prototype → Object.prototype → null` |
| `{}` | `"object"` | `instanceof Object` | `Object.prototype → null` |
| `new Date()` | `"object"` | `instanceof Date` | `Date.prototype → Object.prototype → null` |
| `/regex/` | `"object"` | `instanceof RegExp` | `RegExp.prototype → Object.prototype → null` |
| `new Map()` | `"object"` | `instanceof Map` | `Map.prototype → Object.prototype → null` |
| `new Set()` | `"object"` | `instanceof Set` | `Set.prototype → Object.prototype → null` |
| `new Promise(r => r)` | `"object"` | `instanceof Promise` | `Promise.prototype → Object.prototype → null` |
| `new Error()` | `"object"` | `instanceof Error` | `Error.prototype → Object.prototype → null` |
| `function() {}` | `"function"` | `instanceof Function` | `Function.prototype → Object.prototype → null` |
| `() => {}` | `"function"` | `instanceof Function` | `Function.prototype → Object.prototype → null` |
| `class User {}` | `"function"` | `instanceof Function` | `Function.prototype → Object.prototype → null` |
| `new User()` | `"object"` | `instanceof User` | `User.prototype → Object.prototype → null` |
| `new Number(5)` | `"object"` | `instanceof Number` | `Number.prototype → Object.prototype → null` |
| `new String("x")` | `"object"` | `instanceof String` | `String.prototype → Object.prototype → null` |
| `new Boolean(true)` | `"object"` | `instanceof Boolean` | `Boolean.prototype → Object.prototype → null` |
| `new Array()` | `"object"` | `instanceof Array` | `Array.prototype → Object.prototype → null` |


```jsx
 Object.prototype
   ↑
   ├── Array.prototype
   ├── Function.prototype
   ├── Date.prototype
   ├── Map.prototype
   ├── Set.prototype
   ├── Error.prototype
   └── User.prototype (custom class)
```
