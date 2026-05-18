# EventTarget

`EventTarget` is a JavaScript interface that provides the foundation of the browser event system.

## Core Methods

### addEventListener()
Every event listener receives an `Event` object.

```js
button.addEventListener("click", (event) => {
  console.log(event);
});
```


### removeEventListener()
```js
function handleClick() {
  console.log("clicked");
}

button.addEventListener("click", handleClick);

button.removeEventListener("click", handleClick);
```

### dispatchEvent()
```js
const event = new Event("hello");

document.dispatchEvent(event);
```

# Event Interface

- ```Native```  events are events that are created and fired by the browser (or the operating system) in response to real user interactions or system changes.
- ```Synthetic``` events are events that are manually created and dispatched using JavaScript code.

```
Event Interfaces
├── UIEvent
│   ├── MouseEvent
│   ├── KeyboardEvent
│   ├── InputEvent
│   ├── FocusEvent
│   └── WheelEvent
│
├── SubmitEvent
├── CustomEvent
├── MessageEvent
├── ErrorEvent
└── PopStateEvent
```

## Creating Synthetic Events
```js
const event = new Event("custom");

document.dispatchEvent(event);
```

## CustomEvent
```js
document.addEventListener("user-login", (event) => {
  console.log(event.detail);
});

document.dispatchEvent(
  new CustomEvent("user-login", {
    detail: {
      id: 1,
      name: "Sam"
    }
  })
);
```
