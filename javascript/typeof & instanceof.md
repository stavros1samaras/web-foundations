| Expression   | `typeof`  | `instanceof`  | Prototype Chain |
|--------------|------------------|--------------------|------------------|
| `42` | `"number"` | — | (primitive → no prototype chain) |
| `"text"` | `"string"` | — | (primitive → no prototype chain) |
| `true` | `"boolean"` | — | (primitive → no prototype chain) |
| `Symbol("id")` | `"symbol"` | — | (primitive → no prototype chain) |
| `42n` | `"bigint"` | — | (primitive → no prototype chain) |
| `undefined` | `"undefined"` | — | (no object / no prototype chain) |
| `null` | ⚠️ `"object"` | — | (no prototype chain) |
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
