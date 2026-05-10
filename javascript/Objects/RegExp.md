# JavaScript RegExp

## Instance Methods (Prototype)

| Syntax | Description | Example | Output |
|---|---|---|---|
| `.test()` | Tests if a string matches the regex | `/abc/.test("abcdef")` | `true` |
| `.exec()` | Executes a search and returns match info | `/a(b)c/.exec("abc")` | `["abc","b"]` |
| `.toString()` | Returns regex as a string | `/abc/i.toString()` | `"/abc/i"` |
| `.compile()` | Recompiles the regex (rarely used) | `/abc/.compile("xyz","g")` | `/xyz/g` |


## Instance Properties

| Property | Description | Example | Output |
|---|---|---|---|
| `.source` | Text of the pattern | `/abc/i.source` | `"abc"` |
| `.flags` | Regex flags | `/abc/gi.flags` | `"gi"` |
| `.global` | Boolean indicating `g` flag | `/abc/g.global` | `true` |
| `.ignoreCase` | Boolean indicating `i` flag | `/abc/i.ignoreCase` | `true` |
| `.multiline` | Boolean indicating `m` flag | `/abc/m.multiline` | `true` |
| `.dotAll` | Boolean indicating `s` flag | `/abc/s.dotAll` | `true` |
| `.sticky` | Boolean indicating `y` flag | `/abc/y.sticky` | `true` |
| `.unicode` | Boolean indicating `u` flag | `/abc/u.unicode` | `true` |
| `.lastIndex` | Index at which to start next match | `/abc/g`.lastIndex | `0` |
