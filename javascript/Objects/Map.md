# JavaScript Map

## Static Methods

| Syntax | Description | Example | Output |
|---|---|---|---|
| `new Map()` | Creates a new Map | `new Map([["a",1],["b",2]])` | `Map(2) {"a" => 1, "b" => 2}` |

> Note: Map has almost no static methods besides the constructor.

---

## Instance Methods (Prototype)

| Syntax | Description | Example | Output |
|---|---|---|---|
| `.set()` | Adds or updates a key-value pair | `m.set("c",3)` | `Map {...}` |
| `.get()` | Returns the value of a key | `m.get("a")` | `1` |
| `.has()` | Checks if a key exists | `m.has("b")` | `true` |
| `.delete()` | Removes a key-value pair | `m.delete("a")` | `true` |
| `.clear()` | Removes all key-value pairs | `m.clear()` | `Map(0) {}` |
| `.keys()` | Returns an iterator of keys | `Array.from(m.keys())` | `["a","b"]` |
| `.values()` | Returns an iterator of values | `Array.from(m.values())` | `[1,2]` |
| `.entries()` | Returns an iterator of [key, value] pairs | `Array.from(m.entries())` | `[["a",1],["b",2]]` |
| `.forEach()` | Executes a function for each key-value pair | `m.forEach((v,k)=>console.log(k,v))` | `a 1` `b 2` |

---

## Instance Properties

| Property | Description | Example | Output |
|---|---|---|---|
| `.size` | Returns the number of key-value pairs | `m.size` | `2` |
