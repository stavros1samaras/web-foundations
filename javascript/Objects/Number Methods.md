# JavaScript Number

## Static Methods

| Syntax | Description | Example | Output |
|---|---|---|---|
| `Number(value)` | Converts a value to a number | `Number("123")` | `123` |
| `Number.isNaN()` | Checks if a value is `NaN` | `Number.isNaN(NaN)` | `true` |
| `Number.isInteger()` | Checks if a value is an integer | `Number.isInteger(10)` | `true` |
| `Number.parseInt()` | Converts a string to an integer | `Number.parseInt("42px")` | `42` |
| `Number.parseFloat()` | Converts a string to a float | `Number.parseFloat("3.14px")` | `3.14` |



## Instance Methods (Prototype)

| Syntax | Description | Example | Output |
|---|---|---|---|
| `.toFixed()` | Formats a number with fixed decimals | `(3.14159).toFixed(2)` | `"3.14"` |
| `.toString()` | Converts a number to a string | `(123).toString()` | `"123"` |
| `.toPrecision()` | Formats a number to a specific length | `(3.14159).toPrecision(3)` | `"3.14"` |
| `.valueOf()` | Returns the primitive number value | `(123).valueOf()` | `123` |
| `.toExponential()` | Converts to exponential notation | `(12345).toExponential(2)` | `"1.23e+4"` |
| `.toLocaleString()` | Formats number using locale rules | `(1000000).toLocaleString()` | `"1,000,000"` |


## Static Properties

| Property | Description | Example | Output |
|---|---|---|---|
| `Number.MAX_VALUE` | Largest possible number | `Number.MAX_VALUE` | `1.7976931348623157e+308` |
| `Number.MIN_VALUE` | Smallest positive number | `Number.MIN_VALUE` | `5e-324` |
| `Number.MAX_SAFE_INTEGER` | Largest safe integer | `Number.MAX_SAFE_INTEGER` | `9007199254740991` |
| `Number.MIN_SAFE_INTEGER` | Smallest safe integer | `Number.MIN_SAFE_INTEGER` | `-9007199254740991` |
| `Number.POSITIVE_INFINITY` | Represents infinity | `Number.POSITIVE_INFINITY` | `Infinity` |
| `Number.NEGATIVE_INFINITY` | Represents negative infinity | `Number.NEGATIVE_INFINITY` | `-Infinity` |
| `Number.NaN` | Represents “Not a Number” | `Number.NaN` | `NaN` |

