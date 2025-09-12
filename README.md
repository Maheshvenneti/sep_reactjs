# sep_reactjs

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