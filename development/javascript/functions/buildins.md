# JavaScript Global Functions

## Function Properties (Global Methods)

| Syntax | Description | Example | Output |
|---|---|---|---|
| `eval()` | Executes a string as JavaScript code (unsafe) | `eval("2 + 2")` | `4` |
| `isFinite()` | Checks if value is a finite number | `isFinite(10)` | `true` |
| `isNaN()` | Checks if value is NaN (after coercion) | `isNaN("hello")` | `true` |
| `parseFloat()` | Parses string into floating point number | `parseFloat("3.14px")` | `3.14` |
| `parseInt()` | Parses string into integer (supports radix) | `parseInt("101", 2)` | `5` |
| `encodeURI()` | Encodes a full URI | `encodeURI("https://a b.com")` | `"https://a%20b.com"` |
| `encodeURIComponent()` | Encodes URI component (strict encoding) | `encodeURIComponent("a b&c")` | `"a%20b%26c"` |
| `decodeURI()` | Decodes a full URI | `decodeURI("https://a%20b.com")` | `"https://a b.com"` |
| `decodeURIComponent()` | Decodes URI component | `decodeURIComponent("a%20b%26c")` | `"a b&c"` |


---

## Notes

- `eval()` should be avoided in modern JavaScript due to security risks.
- Prefer `Number.isNaN()` over global `isNaN()`.
- Prefer `encodeURIComponent()` for query parameters.
