# JavaScript (JS)

## Introduction

JavaScript is a **high-level, interpreted programming language** primarily used to add interactivity and dynamic behavior to web applications. It is one of the core technologies of web development alongside **HTML and CSS**.

JavaScript can run in:

* Web browsers
* Servers (Node.js)
* Mobile applications
* Desktop applications

Modern JavaScript is standardized by **ECMAScript (ES)**.

Common uses include:

* DOM manipulation
* Event handling
* Form validation
* API communication
* Building full-stack applications

---

# Adding JavaScript to HTML

JavaScript can be added to HTML in three ways.

---

## Inline JavaScript

JavaScript written directly inside HTML elements.

```html
<button onclick="alert('Hello World')">Click Me</button>
```

Disadvantages:

* Difficult to maintain
* Not reusable

---

## Internal JavaScript

JavaScript written inside `<script>` tags in an HTML file.

```html
<script>
    console.log("Hello JavaScript");
</script>
```

---

## External JavaScript

JavaScript written in a separate `.js` file.

```html
<script src="script.js"></script>
```

Example:

```javascript
console.log("External JavaScript file");
```

Advantages:

* Reusable
* Cleaner HTML
* Better project organization

---

# Variables

Variables store data values.

JavaScript provides three keywords for declaring variables.

```
var
let
const
```

---

## var

Older method of declaring variables.

```javascript
var name = "John";
```

Issues:

* Function scoped
* Allows redeclaration
* Can cause bugs

---

## let

Block-scoped variable introduced in ES6.

```javascript
let age = 20;
```

Features:

* Block scope
* Can be reassigned
* Cannot be redeclared in the same scope

---

## const

Constant variable that cannot be reassigned.

```javascript
const pi = 3.14159;
```

Notes:

* Must be initialized during declaration
* Block scoped

---

# Data Types

JavaScript has two main categories of data types.

---

## Primitive Data Types

Primitive types store single values.

| Type      | Example     |
| --------- | ----------- |
| String    | `"Hello"`   |
| Number    | `42`        |
| Boolean   | `true`      |
| Undefined | `undefined` |
| Null      | `null`      |
| BigInt    | `123n`      |
| Symbol    | `Symbol()`  |

Example:

```javascript
let name = "Manish";
let age = 21;
let isStudent = true;
```

---

## Non-Primitive Data Types

Also called **reference types**.

Examples:

* Objects
* Arrays
* Functions

Example:

```javascript
let user = {
    name: "Manish",
    age: 21
};
```

---

# Operators

Operators perform operations on variables and values.

---

## Arithmetic Operators

```
+
-
*
/
%
**
```

Example:

```javascript
let a = 10;
let b = 3;

console.log(a + b);
console.log(a % b);
```

---

## Comparison Operators

```
==
===
!=
!==
>
<
>=
<=
```

Example:

```javascript
console.log(5 == "5");   // true
console.log(5 === "5");  // false
```

---

## Logical Operators

```
&&
||
!
```

Example:

```javascript
let age = 18;

if (age >= 18 && age < 60) {
    console.log("Eligible");
}
```

---

# Conditional Statements

Conditional statements control program flow.

---

## if Statement

```javascript
let age = 20;

if (age >= 18) {
    console.log("Adult");
}
```

---

## if...else

```javascript
if (age >= 18) {
    console.log("Adult");
} else {
    console.log("Minor");
}
```

---

## else if

```javascript
if (score >= 90) {
    console.log("A");
} else if (score >= 75) {
    console.log("B");
} else {
    console.log("C");
}
```

---

## switch Statement

Used when checking multiple values.

```javascript
let day = 3;

switch(day) {
    case 1:
        console.log("Monday");
        break;

    case 2:
        console.log("Tuesday");
        break;

    default:
        console.log("Invalid day");
}
```

---

# Loops

Loops allow repeated execution of code.

---

## for Loop

```javascript
for (let i = 0; i < 5; i++) {
    console.log(i);
}
```

---

## while Loop

```javascript
let i = 0;

while (i < 5) {
    console.log(i);
    i++;
}
```

---

## do...while Loop

```javascript
let i = 0;

do {
    console.log(i);
    i++;
} while (i < 5);
```

---

# Functions

Functions are reusable blocks of code.

---

## Function Declaration

```javascript
function greet() {
    console.log("Hello");
}
```

---

## Function with Parameters

```javascript
function add(a, b) {
    return a + b;
}

console.log(add(2, 3));
```

---

## Arrow Functions

Introduced in ES6.

```javascript
const add = (a, b) => {
    return a + b;
};
```

Short version:

```javascript
const add = (a, b) => a + b;
```

---

# Arrays

Arrays store multiple values in a single variable.

```javascript
let numbers = [1, 2, 3, 4];
```

Access element:

```javascript
console.log(numbers[0]);
```

---

## Common Array Methods

### push()

Adds element to end.

```javascript
numbers.push(5);
```

---

### pop()

Removes last element.

```javascript
numbers.pop();
```

---

### shift()

Removes first element.

```javascript
numbers.shift();
```

---

### unshift()

Adds element to beginning.

```javascript
numbers.unshift(0);
```

---

### map()

Creates a new array.

```javascript
let doubled = numbers.map(n => n * 2);
```

---

### filter()

Filters elements.

```javascript
let even = numbers.filter(n => n % 2 === 0);
```

---

### reduce()

Reduces array to a single value.

```javascript
let sum = numbers.reduce((acc, curr) => acc + curr, 0);
```

---

# Objects

Objects store data in key-value pairs.

```javascript
let person = {
    name: "Manish",
    age: 21
};
```

Access property:

```javascript
console.log(person.name);
```

---

# DOM (Document Object Model)

The DOM represents HTML as a tree structure.

JavaScript can manipulate the DOM to change webpage content dynamically.

---

## Selecting Elements

### getElementById

```javascript
document.getElementById("title");
```

---

### querySelector

```javascript
document.querySelector(".className");
```

---

### querySelectorAll

```javascript
document.querySelectorAll("p");
```

---

# Event Handling

Events allow interaction with user actions.

Examples:

* click
* submit
* keypress
* mouseover

Example:

```javascript
button.addEventListener("click", function() {
    console.log("Button clicked");
});
```

---

# ES6 Features

Modern JavaScript introduced several improvements.

---

## Template Literals

```javascript
let name = "Manish";

console.log(`Hello ${name}`);
```

---

## Destructuring

```javascript
const user = { name: "Manish", age: 21 };

const { name, age } = user;
```

---

## Spread Operator

```javascript
let arr1 = [1,2];
let arr2 = [...arr1, 3,4];
```

---

## Rest Operator

```javascript
function sum(...numbers) {
    return numbers.reduce((a,b) => a + b);
}
```

---

# Asynchronous JavaScript

JavaScript is **single-threaded but asynchronous**.

---

## Callbacks

```javascript
function fetchData(callback) {
    setTimeout(() => {
        callback("Data received");
    }, 1000);
}
```

---

## Promises

```javascript
let promise = new Promise((resolve, reject) => {
    resolve("Success");
});
```

Usage:

```javascript
promise.then(result => console.log(result));
```

---

## Async / Await

Cleaner way to handle asynchronous code.

```javascript
async function fetchData() {
    let response = await fetch("api-url");
    let data = await response.json();
    console.log(data);
}
```

---

# Error Handling

JavaScript provides `try...catch`.

```javascript
try {
    let x = y;
} catch (error) {
    console.log(error);
}
```

---

# Modules

Modules allow code splitting.

Export:

```javascript
export function add(a, b) {
    return a + b;
}
```

Import:

```javascript
import { add } from "./math.js";
```

---

# Best Practices

* Use `const` by default
* Use `let` when reassignment is required
* Avoid `var`
* Write modular code
* Follow consistent naming conventions
* Handle errors properly
* Use modern ES6+ features

---

# Conclusion

JavaScript is a powerful programming language used for building modern web applications. Mastering concepts such as **functions, objects, DOM manipulation, asynchronous programming, and ES6 features** is essential for becoming a proficient web developer.

