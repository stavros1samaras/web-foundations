# JavaScript Boolean

## Static Methods

| Syntax | Description | Example | Output |
|---|---|---|---|
| `Boolean(value)` | Converts a value to boolean | `Boolean(1)` | `true` |
| `Boolean()` | Converts falsy/truthy values to boolean | `Boolean(0)` | `false` |
| `Boolean()` | Common truthy/falsy conversion utility | `Boolean("hello")` | `true` |


## Instance Methods (Prototype)

> ⚠️ Note: Booleans in JavaScript are primitives and **do not have useful instance methods** in everyday usage.

| Syntax | Description | Example | Output |
|---|---|---|---|
| `.valueOf()` | Returns primitive boolean value | `(true).valueOf()` | `true` |
| `.toString()` | Converts boolean to string | `(true).toString()` | `"true"` |


## Important Concept

JavaScript values are automatically treated as **truthy or falsy**:

### Falsy values:
- `false`
- `0`
- `""` (empty string)
- `null`
- `undefined`
- `NaN`

### Everything else is truthy:
```js
Boolean("hello") // true
Boolean(123)     // true
Boolean([])      // true
Boolean({})      // true
