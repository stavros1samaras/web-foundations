# JavaScript Set

## Static Methods

## Instance Methods (Prototype)

| Syntax | Description | Example | Output |
|---|---|---|---|
| `.add()` | Adds a value to the set | `s.add(4)` | `Set {...}` |
| `.delete()` | Removes a value | `s.delete(2)` | `true` |
| `.has()` | Checks if a value exists | `s.has(3)` | `true` |
| `.clear()` | Removes all values | `s.clear()` | `Set(0) {}` |
| `.keys()` | Returns an iterator of values (same as `.values()`) | `Array.from(s.keys())` | `[1,2,3]` |
| `.values()` | Returns an iterator of values | `Array.from(s.values())` | `[1,2,3]` |
| `.entries()` | Returns an iterator of [value, value] pairs | `Array.from(s.entries())` | `[[1,1],[2,2],[3,3]]` |
| `.forEach()` | Executes a function for each value | `s.forEach(v => console.log(v))` | `1 2 3` |


## Instance Properties

| Property | Description | Example | Output |
|---|---|---|---|
| `.size` | Number of values in the set | `s.size` | `3` |
