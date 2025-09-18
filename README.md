# sep_reactjs

## Variables

JavaScript provides three ways to declare variables:

```js
// var: function-scoped
var name = 'mahes';
var name = 'suresh'; // Redeclaration allowed

// let: block-scoped
let count = 10;
count = 20; // Re-assignment allowed

// const: block-scoped, cannot be re-assigned
const age = 18;
// age = 22; // Error: Assignment to constant variable
```

## Scope

- **Function Scope** (with `var`):
```js
function test() {
  var x = 10;
  // x is accessible here
}
// x is NOT accessible here
```

- **Block Scope** (with `let` and `const`):
```js
{
  let y = 20;
  const z = 30;
  // y and z are accessible here
}
// y and z are NOT accessible here
```

## Data Types

JavaScript has two main categories of data types:

### Primitive Data Types

```js
// 1. String
let str = "string";

// 2. Number
let num = 1234;

// 3. Boolean
let isActive = true; // or false

// 4. Undefined
let a;
console.log(a); // undefined

// 5. Null
let b = null; // intentional empty value
```

### Non-Primitive Data Types

```js
// Object
let address = {
  city: "Hyderabad",
  state: "TS"
};

// Array
let fruits = ["apple", "banana", "cherry"];

// Function
function fire() {
  console.log("function fire");
}
fire();
```


# Operators

Operators in JavaScript are special symbols or keywords used to perform operations on operands (values and variables). They are essential for manipulating data and controlling logic in your code. JavaScript supports several types of operators, including comparison, arithmetic, assignment, logical, and more.

Below are some of the most commonly used operators:

## Comparison Operators

```js
// == or ===
// Result is always true or false

// Loose equality (==): compares values only
console.log(a == b); // true

// Strict equality (===): compares both value and type
console.log(a === b); // false

// Not equal (!=) and strict not equal (!==)
console.log(a != b);   // false
console.log(a !== b);  // true

// Greater than, greater than or equal to
console.log(a > b);    // false
console.log(a >= b);   // true
```

## Arithmetic Operators

```js
console.log(a + b); // Addition
console.log(a - b); // Subtraction
console.log(a * b); // Multiplication
console.log(a / b); // Division
console.log(a % b); // Remainder
```

## Ternary Operator

A shorter way to write if-else:

```js
let age = 17;
let major = (age >= 18) ? "Yes" : "No";
console.log(major);
```

Equivalent if-else:

```js
if (age >= 18) {
  major = "Yes";
} else {
  major = "No";
}
```

## Assignment Operators

```js
let num = 10;
// num += 5; // num = num + 5
num -= 5;   // num = num - 5
console.log(num);
```

## Logical Operators

```js
let age = 20;

// AND (&&)
console.log(age > 18 && age < 25); // true

// OR (||)
console.log(age > 18 || age < 25); // true
```

## Loops

Loops are used to execute a block of code multiple times. JavaScript provides several types of loops:

### for Loop

```js
for (let i = 0; i < 5; i++) {
  console.log(i); // Prints 0 to 4
}
```

### while Loop

```js
let count = 0;
while (count < 3) {
  console.log(count); // Prints 0, 1, 2
  count++;
}
```

### do...while Loop

```js
let num = 0;
do {
  console.log(num); // Prints 0, 1, 2
  num++;
} while (num < 3);
```

### for...of Loop (for arrays)

```js
const fruits = ["apple", "banana", "cherry"];
for (const fruit of fruits) {
  console.log(fruit); // Prints each fruit
}
```
### for...in Loop (for objects)

```js
const address = { city: "Hyderabad", state: "TS" };
for (const key in address) {
  console.log(key, address[key]); // Prints key and value
}
```