# JavaScript typeof / instanceof / Prototype Chain

| Expression | typeof | instanceof | Prototype Chain |
|------------|--------|------------|-----------------|
| const num = 42 | "number" | — | No prototype chain |
| const str = "text" | "string" | — | No prototype chain |
| const bool = true | "boolean" | — | No prototype chain |
| const sym = Symbol("id") | "symbol" | — | No prototype chain |
| const big = 42n | "bigint" | — | No prototype chain |
| const und = undefined | "undefined" | — | No prototype chain |
| const nul = null | "object" | — | No prototype chain |
| const arr = new Array() | "object" | arr instanceof Array → true | Array.prototype → Object.prototype → null |
| const obj = {} | "object" | obj instanceof Object → true | Object.prototype → null |
| const date = new Date() | "object" | date instanceof Date → true | Date.prototype → Object.prototype → null |
| const regex = /regex/ | "object" | regex instanceof RegExp → true | RegExp.prototype → Object.prototype → null |
| const map = new Map() | "object" | map instanceof Map → true | Map.prototype → Object.prototype → null |
| const set = new Set() | "object" | set instanceof Set → true | Set.prototype → Object.prototype → null |
| const promise = new Promise(r => r()) | "object" | promise instanceof Promise → true | Promise.prototype → Object.prototype → null |
| const err = new Error() | "object" | err instanceof Error → true | Error.prototype → Object.prototype → null |
| const fn = function() {} | "function" | fn instanceof Function → true | Function.prototype → Object.prototype → null |
| const arrow = () => {} | "function" | arrow instanceof Function → true | Function.prototype → Object.prototype → null |
| const user = new (function User() {})() | "object" | user instanceof Object → true | Object.prototype → null |
| const numObj = new Number(5) | "object" | numObj instanceof Number → true | Number.prototype → Object.prototype → null |
| const strObj = new String("x") | "object" | strObj instanceof String → true | String.prototype → Object.prototype → null |
| const boolObj = new Boolean(true) | "object" | boolObj instanceof Boolean → true | Boolean.prototype → Object.prototype → null |

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
