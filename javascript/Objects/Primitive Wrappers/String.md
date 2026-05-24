# JavaScript String Methods

## Static Methods

| Syntax | Description | Example | Output |
|---|---|---|---|
| `String(value)` | Converts a value to a string | `String(123)` | `"123"` |
| `String.fromCharCode()` | Creates a string from Unicode values | `String.fromCharCode(72, 73)` | `"HI"` |
| `String.fromCodePoint()` | Creates a string from Unicode code points | `String.fromCodePoint(128512)` | `"😀"` |
| `String.raw()` | Returns a raw string without escaping characters | ``String.raw`Hello\nWorld` `` | `"Hello\\nWorld"` |


## Prototype Methods

| Syntax | Description | Example | Output |
|---|---|---|---|
| `.toUpperCase()` | Converts text to uppercase | `"hello".toUpperCase()` | `"HELLO"` |
| `.toLowerCase()` | Converts text to lowercase | `"HELLO".toLowerCase()` | `"hello"` |
| `.trim()` | Removes spaces from both ends | `" hello ".trim()` | `"hello"` |
| `.includes()` | Checks if text exists inside a string | `"hello".includes("ell")` | `true` |
| `.startsWith()` | Checks if a string starts with specific text | `"hello".startsWith("he")` | `true` |
| `.endsWith()` | Checks if a string ends with specific text | `"hello".endsWith("lo")` | `true` |
| `.replace()` | Replaces part of a string | `"hello".replace("h", "H")` | `"Hello"` |
| `.replaceAll()` | Replaces all matches in a string | `"a-a-a".replaceAll("-", "_")` | `"a_a_a"` |
| `.slice()` | Extracts part of a string | `"hello".slice(1, 4)` | `"ell"` |
| `.substring()` | Returns part of a string using indexes | `"hello".substring(1, 4)` | `"ell"` |
| `.split()` | Splits a string into an array | `"a,b,c".split(",")` | `["a","b","c"]` |
| `.concat()` | Combines strings together | `"Hello".concat(" World")` | `"Hello World"` |
| `.repeat()` | Repeats a string multiple times | `"ha".repeat(3)` | `"hahaha"` |
| `.charAt()` | Returns a character at a specific index | `"hello".charAt(1)` | `"e"` |
| `.indexOf()` | Finds the first index of text | `"hello".indexOf("l")` | `2` |
| `.lastIndexOf()` | Finds the last index of text | `"hello".lastIndexOf("l")` | `3` |
| `.match()` | Searches using a regex pattern | `"hello".match(/l/g)` | `["l","l"]` |
| `.search()` | Returns the position of a regex match | `"hello".search(/l/)` | `2` |
| `.padStart()` | Adds characters at the beginning | `"5".padStart(3, "0")` | `"005"` |
| `.padEnd()` | Adds characters at the end | `"5".padEnd(3, "0")` | `"500"` |
| `.localeCompare()` | Compares two strings alphabetically | `"a".localeCompare("b")` | `-1` |
| `.valueOf()` | Returns the primitive string value | `"hello".valueOf()` | `"hello"` |
| `.toString()` | Returns the string as text | `"hello".toString()` | `"hello"` |

