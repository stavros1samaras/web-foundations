# JavaScript JSON

## Static Methods

| Syntax | Description | Example | Output |
|---|---|---|---|
| `JSON.stringify()` | Converts JavaScript value to JSON string | `JSON.stringify({a:1})` | `'{"a":1}'` |
| `JSON.parse()` | Converts JSON string to JavaScript value | `JSON.parse('{"a":1}')` | `{ a: 1 }` |


## Important Concept

### 🔄 JSON is a data format, not a JavaScript object system

- JSON = text format (string)
- JavaScript object = in-memory structure

```js
const obj = { name: "Alex" };

const json = JSON.stringify(obj);
// '{"name":"Alex"}'

const back = JSON.parse(json);
// { name: "Alex" }
```

## ⚠️ JSON limitations

JSON does NOT support:

- functions
- undefined
- Symbols
- BigInt
