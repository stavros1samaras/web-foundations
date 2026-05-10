# JavaScript Object

## Static Methods

| Syntax | Description | Example | Output |
|---|---|---|---|
| `Object()` | Creates an object wrapper or converts value | `Object(123)` | `Number {123}` |
| `Object.keys()` | Returns object keys | `Object.keys({a:1})` | `["a"]` |
| `Object.values()` | Returns object values | `Object.values({a:1})` | `[1]` |
| `Object.entries()` | Returns key-value pairs | `Object.entries({a:1})` | `[["a",1]]` |
| `Object.fromEntries()` | Converts entries to object | `Object.fromEntries([["a",1]])` | `{a:1}` |
| `Object.assign()` | Copies properties between objects | `Object.assign({}, {a:1})` | `{a:1}` |
| `Object.hasOwn()` | Checks own property existence | `Object.hasOwn({a:1},"a")` | `true` |
| `Object.freeze()` | Makes object immutable | `Object.freeze(obj)` | frozen object |
| `Object.seal()` | Prevents adding/removing props | `Object.seal(obj)` | sealed object |
| `Object.create()` | Creates object with prototype | `Object.create(null)` | `{}` |
| `Object.defineProperty()` | Defines a property | `Object.defineProperty(obj,"a",{value:1})` | object |
| `Object.getOwnPropertyDescriptor()` | Gets property details | `Object.getOwnPropertyDescriptor(obj,"a")` | descriptor |
| `Object.getOwnPropertyNames()` | Gets all string keys | `Object.getOwnPropertyNames(obj)` | `["a"]` |
| `Object.getOwnPropertySymbols()` | Gets symbol keys | `Object.getOwnPropertySymbols(obj)` | `[Symbol()]` |
| `Object.getPrototypeOf()` | Gets prototype | `Object.getPrototypeOf(obj)` | prototype |
| `Object.setPrototypeOf()` | Sets prototype | `Object.setPrototypeOf(obj, proto)` | object |


## Instance Methods (Prototype)

| Syntax | Description | Example | Output |
|---|---|---|---|
| `.toString()` | Returns string representation | `{a:1}.toString()` | `"[object Object]"` |
| `.valueOf()` | Returns primitive value | `obj.valueOf()` | object itself |
| `.hasOwnProperty()` | Checks own property | `{a:1}.hasOwnProperty("a")` | `true` |
| `.isPrototypeOf()` | Checks prototype chain | `proto.isPrototypeOf(obj)` | `true` |
| `.propertyIsEnumerable()` | Checks if property is enumerable | `obj.propertyIsEnumerable("a")` | `true` |

