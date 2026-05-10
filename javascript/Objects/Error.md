# JavaScript Error


## Instance Methods (Prototype)

| Syntax | Description | Example | Output |
|---|---|---|---|
| `.name` | Returns the error name | `e.name` | `"Error"` |
| `.message` | Returns the error message | `e.message` | `"Something went wrong"` |
| `.toString()` | Returns string representation | `e.toString()` | `"Error: Something went wrong"` |

> Subtypes include `TypeError`, `ReferenceError`, `SyntaxError`, `RangeError`, etc., which inherit the same methods.


## Instance Properties

| Property | Description | Example | Output |
|---|---|---|---|
| `.name` | Error name | `e.name` | `"Error"` |
| `.message` | Error message | `e.message` | `"Something went wrong"` |
| `.stack` | Stack trace (non-standard in some environments) | `e.stack` | `"Error: Something went wrong at ..."` |
