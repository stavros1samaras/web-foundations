# JavaScript Classes Cheat Sheet

## Public Properties

All fields are public by default.

```js
class User {
  name = "Nikos";
}

const u = new User();

console.log(u.name);

u.name = "Maria";
```



## Private Properties (`#`)

```js
class BankAccount {
  #balance = 0;

  deposit(amount) {
    this.#balance += amount;
  }

  showBalance() {
    console.log(this.#balance);
  }
}

const acc = new BankAccount();

acc.deposit(100);

acc.showBalance();
```

This is NOT allowed:

```js
acc.#balance
```



## Constructor

The constructor runs when a new object is created.

```js
class User {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }
}
```

### Creating an object

```js
const u = new User("Nikos", 25);
```


## Methods (Functions inside a class)

```js
class Car {
  start() {
    console.log("The car started");
  }

  stop() {
    console.log("The car stopped");
  }
}
```



## Getters

A getter reads a value like a property.

```js
class User {
  #name = "";

  constructor(name) {
    this.#name = name;
  }

  get name() {
    return this.#name;
  }
}

const u = new User("Maria");

console.log(u.name);
```



## Setters

A setter changes a value like a property.

```js
class User {
  #name = "";

  set name(value) {
    this.#name = value;
  }
}

const u = new User();

u.name = "Anna";
```



## Static Methods

Static methods belong to the class itself, not to objects.

```js
class MathHelper {
  static add(a, b) {
    return a + b;
  }
}

console.log(MathHelper.add(2, 3));
```

### This does NOT work:

```js
const m = new MathHelper();

m.add(); // ERROR
```



## Inheritance (`extends`)

A class can inherit from another class.

```js
class Animal {
  speak() {
    console.log("The animal makes a sound");
  }
}

class Dog extends Animal {
  bark() {
    console.log("Woof woof!");
  }
}

const dog = new Dog();

dog.speak();
dog.bark();
```



## `super()`

Used to call the parent class constructor.

```js
class Animal {
  constructor(name) {
    this.name = name;
  }
}

class Dog extends Animal {
  constructor(name, breed) {
    super(name);

    this.breed = breed;
  }
}
```

## Template

```js
class MyClass {
  // public fields
  value = 0;

  // private fields
  #secret = "";

  // constructor
  constructor(value) {
    this.value = value;
  }

  // getter
  get secret() {
    return this.#secret;
  }

  // setter
  set secret(v) {
    this.#secret = v;
  }

  // methods
  doSomething() {}

  // static methods
  static helper() {}
}
```
