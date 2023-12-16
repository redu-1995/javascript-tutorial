# Javascript tutorial

# JavaScript Variables

# Variables are Containers for Storing Data

JavaScript Variables can be declared in 4 ways:

- Automatically
- Using `var`
- Using `let`
- Using `const`

In this first example, `x`, `y`, and `z` are undeclared variables.

They are automatically declared when first used:

# Example

```jsx
x = 5;
y = 6;
z = x + y;
```

# Note

It is considered good programming practice to always declare variables before use.

From the examples you can guess:

- x stores the value 5
- y stores the value 6
- z stores the value 11

# Example using var

```jsx
var x = 5;
var y = 6;
var z = x + y;
```

# Note

The `var` keyword was used in all JavaScript code from 1995 to 2015.

The `let` and `const` keywords were added to JavaScript in 2015.

The `var` keyword should only be used in code written for older browsers.

# Example using let

```jsx
let x = 5;let y = 6;let z = x + y;
```

# Example using const

```jsx
const x = 5;const y = 6;const z = x + y;
```

# Mixed Example

```jsx
const price1 = 5;const price2 = 6;let total = price1 + price2;
```

The two variables `price1` and `price2` are declared with the `const` keyword.

These are constant values and cannot be changed.

The variable `total` is declared with the `let` keyword.

The value `total` can be changed.

# When to Use var, let, or const?

1. Always declare variables

2. Always use `const` if the value should not be changed

3. Always use `const` if the type should not be changed (Arrays and Objects)

4. Only use `let` if you can't use `const`

5. Only use `var` if you MUST support old browsers.

---

# Just Like Algebra

Just like in algebra, variables hold values:

let x = 5;let y = 6;

Just like in algebra, variables are used in expressions:

let z = x + y;

From the example above, you can guess that the total is calculated to be 11.

# Note

Variables are containers for storing values.

---

---

# JavaScript Identifiers

All JavaScript **variables** must be **identified** with **unique names**.

These unique names are called **identifiers**.

Identifiers can be short names (like x and y) or more descriptive names (age, sum, totalVolume).

The general rules for constructing names for variables (unique identifiers) are:

- Names can contain letters, digits, underscores, and dollar signs.
- Names must begin with a letter.
- Names can also begin with $ and _ (but we will not use it in this tutorial).
- Names are case sensitive (y and Y are different variables).
- Reserved words (like JavaScript keywords) cannot be used as names.

# Note

JavaScript identifiers are case-sensitive.

---

# The Assignment Operator

In JavaScript, the equal sign (`=`) is an "assignment" operator, not an "equal to" operator.

This is different from algebra. The following does not make sense in algebra:

x = x + 5

In JavaScript, however, it makes perfect sense: it assigns the value of x + 5 to x.

(It calculates the value of x + 5 and puts the result into x. The value of x is incremented by 5.)

# Note

The "equal to" operator is written like `==` in JavaScript.

---

# JavaScript Data Types

JavaScript variables can hold numbers like 100 and text values like "John Doe".

In programming, text values are called text strings.

JavaScript can handle many types of data, but for now, just think of numbers and strings.

Strings are written inside double or single quotes. Numbers are written without quotes.

If you put a number in quotes, it will be treated as a text string.

# Example

```jsx
const pi = 3.14;let person = "John Doe";let answer = 'Yes I am!';
```

---

# Declaring a JavaScript Variable

Creating a variable in JavaScript is called "declaring" a variable.

You declare a JavaScript variable with the `var` or the `let` keyword:

var carName;

or:

let carName;

After the declaration, the variable has no value (technically it is `undefined`).

To **assign** a value to the variable, use the equal sign:

carName = "Volvo";

You can also assign a value to the variable when you declare it:

let carName = "Volvo";

In the example below, we create a variable called `carName` and assign the value "Volvo" to it.

Then we "output" the value inside an HTML paragraph with id="demo":

# Example

```c
<p id="demo"></p><script>let carName = "Volvo";document.getElementById("demo").innerHTML = carName;</script>
```

# Note

It's a good programming practice to declare all variables at the beginning of a script.

---

# One Statement, Many Variables

You can declare many variables in one statement.

Start the statement with `let` and separate the variables by **comma**:

# Example

```jsx
let person = "John Doe", carName = "Volvo", price = 200;
```

A declaration can span multiple lines:

# Example

```jsx
let person = "John Doe",carName = "Volvo",price = 200;
```

---

# Value = undefined

In computer programs, variables are often declared without a value. The value can be something that has to be calculated, or something that will be provided later, like user input.

A variable declared without a value will have the value `undefined`.

The variable carName will have the value `undefined` after the execution of this statement:

# Example

```jsx
let carName;
```

---

# Re-Declaring JavaScript Variables

If you re-declare a JavaScript variable declared with `var`, it will not lose its value.

The variable `carName` will still have the value "Volvo" after the execution of these statements:

# Example

```jsx
var carName = "Volvo";var carName;
```

# Note

You cannot re-declare a variable declared with `let` or `const`.

This will not work:

```jsx
let carName = "Volvo";let carName;
```

---

# JavaScript Arithmetic

As with algebra, you can do arithmetic with JavaScript variables, using operators like `=` and `+`:

# Example

```jsx
let x = 5 + 2 + 3;
```

You can also add strings, but strings will be concatenated:

# Example

```jsx
let x = "John" + " " + "Doe";
```

Also try this:

# Example

```jsx
let x = "5" + 2 + 3;
```

# Note

If you put a number in quotes, the rest of the numbers will be treated as strings, and concatenated.

Now try this:

# Example

```jsx
let x = 2 + 3 + "5";
```

---

# JavaScript Dollar Sign $

Since JavaScript treats a dollar sign as a letter, identifiers containing $ are valid variable names:

# Example

```jsx
let $ = "Hello World";let $$$ = 2;let $myMoney = 5;
```

Using the dollar sign is not very common in JavaScript, but professional programmers often use it as an alias for the main function in a JavaScript library.

In the JavaScript library jQuery, for instance, the main function `$` is used to select HTML elements. In jQuery `$("p");` means "select all p elements".

---

# JavaScript Underscore (_)

Since JavaScript treats underscore as a letter, identifiers containing _ are valid variable names:

# Example

```jsx
let _lastName = "Johnson";let _x = 2;let _100 = 5;
```

Using the underscore is not very common in JavaScript, but a convention among professional programmers is to use it as an alias for "private (hidden)" variables.

**Primitive and Non-primitive data-types in JavaScript**

Every Variable has a data type that tells what kind of data is being stored in a variable. There are two types of data types in JavaScript.

- Primitive data types
- Non-primitive data types

**Primitive data types:** The predefined data types provided by JavaScript language are known as primitive data types. Primitive data types are also known as in-built data types.

**Below is a list of Primitive Data Types with proper descriptions and examples:**

**1. [Number](https://www.geeksforgeeks.org/javascript-numbers/):** Number data type in javascript can be used to hold decimal values as well as values without decimals.

- Javascript

```jsx
let x = 250;

let y = 40.5;

console.log("Value of x=" + x);

`console.log("Value of y=" + y);
```

``

---

**Output:**

![https://media.geeksforgeeks.org/wp-content/uploads/20211115201228/numberoutput-300x202.png](https://media.geeksforgeeks.org/wp-content/uploads/20211115201228/numberoutput-300x202.png)

*number output*

**2.** **[String](https://www.geeksforgeeks.org/javascript-strings/):** The string data type in javascript represents a sequence of characters that are surrounded by single or double quotes.

```jsx
let str = 'Hello All';

let str1 = "Welcome to my new house";

console.log("Value of str=" + str);

console.log("Value of str1=" + str1);
```

``

---

**Output:**

![https://media.geeksforgeeks.org/wp-content/uploads/20211115201529/stringoutput-300x124.png](https://media.geeksforgeeks.org/wp-content/uploads/20211115201529/stringoutput-300x124.png)

*string output*

**3. [Undefined](https://www.geeksforgeeks.org/javascript-undefined-property/):** The meaning of undefined is ‘value is not assigned’.

- Javascript

```jsx
console.log("Value of x=" + x);
```

``

---

**Output:**

![https://media.geeksforgeeks.org/wp-content/uploads/20211115204534/undefined-300x149.png](https://media.geeksforgeeks.org/wp-content/uploads/20211115204534/undefined-300x149.png)

*undefined  output*

**4. [Boolean](https://www.geeksforgeeks.org/javascript-boolean/):** The boolean data type can accept only two values i.e. true and false.

- Javascript

```jsx
console.log("value of bool=" + bool);
```

---

**Output:**

![https://media.geeksforgeeks.org/wp-content/uploads/20211115204351/booloutput2-300x165.png](https://media.geeksforgeeks.org/wp-content/uploads/20211115204351/booloutput2-300x165.png)

*boolean output*

**5. [Null](https://www.geeksforgeeks.org/null-in-javascript/):** This data type can hold only one possible value that is null.

- Javascript

```jsx
let x = null;

console.log("Value of x="+ x);
```

---

![https://media.geeksforgeeks.org/wp-content/uploads/20211115165654/null-300x151.png](https://media.geeksforgeeks.org/wp-content/uploads/20211115165654/null-300x151.png)

*null  output*

**6. [BigInt](https://www.geeksforgeeks.org/bigint-in-javascript/):** This data type can represent numbers greater than 253-1 which helps to perform operations on large numbers. The number is specified by writing ‘n’ at the end of the value

- Javascript

```jsx
var bigNum = 123422222222222222222222222222222222222n

console.log(bigNum)
```

---

**Output:**

```
123422222222222222222222222222222222222n
```

**7. [Symbol](https://www.geeksforgeeks.org/javascript-symbol-method/):** This data type is used to create objects which will always be unique. these objects can be created using Symbol constructor.

- Javascript

```jsx
var sym = Symbol("Hello")

console.log(typeof(sym));

console.log(sym);
```

---

**Output:**

![https://media.geeksforgeeks.org/wp-content/uploads/20230306171409/gfg.png](https://media.geeksforgeeks.org/wp-content/uploads/20230306171409/gfg.png)

*Symbol Output*

**Non-primitive data types:** The data types that are derived from primitive data types of the JavaScript language are known as non-primitive data types. It is also known as derived data types or reference data types.

Below is a list of Non-primitive data types.

Non-primitive Data Types

---

[Object](https://www.geeksforgeeks.org/objects-in-javascript/)

---

[Array](https://www.geeksforgeeks.org/arrays-in-javascript/)

---

**Below is a list of Non-primitive Data Types with proper descriptions and examples:**

**1. [Object](https://www.geeksforgeeks.org/javascript-objects/): An object** in Javascript is an entity having properties and methods. Everything is an object in javascript.

How to create an object in javascript:

- **Using Constructor Function to define an object:**

```
// Create an empty generic object
var obj = new Object();

// Create a user defined object
var mycar = new Car();
```

- **Using Literal notations to define an object:**

```
// An empty object
var square = {};

// Here a and b are keys and
// 20 and 30 are values
var circle = {a: 20, b: 30};
```

**Example:**

- Javascript

```jsx
// Creating object with the name person`

let person = {

firstName: "Luiza",

lastName: "Shaikh",

};

// Print the value of object on console`

console.log(person.firstName
+ "  "` `+ person.lastName);
```

``

---

![https://media.geeksforgeeks.org/wp-content/uploads/20211115202538/objectoutput-300x228.png](https://media.geeksforgeeks.org/wp-content/uploads/20211115202538/objectoutput-300x228.png)

*object output*

**2. [Array](https://www.geeksforgeeks.org/arrays-in-javascript/):** With the help of an array, we can store more than one element under a single name.

**Ways to declare a** **single-dimensional array:**

```
// Call it with no arguments
var a = new Array();

// Call it with single numeric argument
var b = new Array(10);

// Explicitly specify two or
// more array elements
var d = new Array(1, 2, 3, "Hello");
```

**Example:**

Javascript

```jsx
var a = new Array();

var b = new Array(10);`

var d = new Array(1, 2, 3, "Hello");

console.log("value of a=" + a);

console.log("value of b" + b);

console.log("value of d=" + d);
```

---

**Output:**

**Note:** JavaScript does not support two-dimensional arrays. but we can do this by creating an array of an array.

**Difference between Primitive vs Non-Primitive:**

| Primitive | Non-Primitive |
| --- | --- |
| Primitive Data types are predefined. | Non-Primitive data types are created by the programmer |
| Primitive Data types will have certain values. | Non-Primitive data types can be NULL. |
| Size depends on the type of data structure. | Size is not fixed |
| Examples are numbers and strings. | Examples are Array and Linked List. |
| It can start with a lowercase. | It can start with uppercase. |

# JavaScript Operators

The **Addition Operator** 
**+** adds numbers:

The **Assignment Operator** 
**=** assigns a value to a variable.

![https://www.w3schools.com/js/img_operators.jpg](https://www.w3schools.com/js/img_operators.jpg)

---

# JavaScript Assignment

The **Assignment Operator** (`=`) assigns a value to a variable:

# Assignment Examples

let x = 10;

```jsx
// Assign the value 5 to x 
let x = 5;
// Assign the value 2 to y 
let y = 2;
// Assign the value x + y to z:
let z = x + y;
```

---

# JavaScript Addition

The **Addition Operator** (`+`) adds numbers:

# Adding

```jsx
let x = 5;
let y = 2;
let z = x + y;
```

# JavaScript Multiplication

The **Multiplication Operator** (`*`) multiplies numbers:

# Multiplying

```jsx
let x = 5;
let y = 2;
let z = x * y;
```

---

# Types of JavaScript Operators

There are different types of JavaScript operators:

- Arithmetic Operators
- Assignment Operators
- Comparison Operators
- String Operators
- Logical Operators
- Bitwise Operators
- Ternary Operators
- Type Operators

---

# JavaScript Arithmetic Operators

**Arithmetic Operators** are used to perform arithmetic on numbers:

# Arithmetic Operators Example

| Operator | Description |
| --- | --- |
| + | Addition |
| - | Subtraction |
| * | Multiplication |
| ** | Exponentiation (https://www.w3schools.com/js/js_2016.asp) |
| / | Division |
| % | Modulus (Division Remainder) |
| ++ | Increment |
| -- | Decrement |

# Note

Arithmetic operators are fully described in the **[JS Arithmetic](https://www.w3schools.com/js/js_arithmetic.asp)** chapter.

---

---

# JavaScript Assignment Operators

Assignment operators assign values to JavaScript variables.

The **Addition Assignment Operator** (`+=`) adds a value to a variable.

# Assignment

let x = 10;x += 5;

[Try it Yourself »](https://www.w3schools.com/js/tryit.asp?filename=tryjs_oper_plusequal)

| Operator | Example | Same As |
| --- | --- | --- |
| = | x = y | x = y |
| += | x += y | x = x + y |
| -= | x -= y | x = x - y |
| *= | x *= y | x = x * y |
| /= | x /= y | x = x / y |
| %= | x %= y | x = x % y |
| **= | x **= y | x = x ** y |

# Note

Assignment operators are fully described in the **[JS Assignment](https://www.w3schools.com/js/js_assignment.asp)** chapter.

---

# JavaScript Comparison Operators

| Operator | Description |
| --- | --- |
| == | equal to |
| === | equal value and equal type |
| != | not equal |
| !== | not equal value or not equal type |
| > | greater than |
| < | less than |
| >= | greater than or equal to |
| <= | less than or equal to |
| ? | ternary operator |

# Note

Comparison operators are fully described in the **[JS Comparisons](https://www.w3schools.com/js/js_comparisons.asp)** chapter.

---

# JavaScript String Comparison

All the comparison operators above can also be used on strings:

# Example

```jsx
let text1 = "A";let text2 = "B";let result = text1 < text2;
```

Note that strings are compared alphabetically:

# Example

```jsx
let text1 = "20";let text2 = "5";let result = text1 < text2;
```

---

# JavaScript String Addition

The `+` can also be used to add (concatenate) strings:

# Example

```jsx
let text1 = "John";let text2 = "Doe";let text3 = text1 + " " + text2;
```

The `+=` assignment operator can also be used to add (concatenate) strings:

# Example

```jsx
let text1 = "What a very ";text1 += "nice day";
```

The result of text1 will be:

`What a very nice day`

# Note

When used on strings, the + operator is called the concatenation operator.

---

# Adding Strings and Numbers

Adding two numbers, will return the sum, but adding a number and a string will return a string:

# Example

```jsx
let x = 5 + 5;let y = "5" + 5;let z = "Hello" + 5;
```

The result of *x*, *y*, and *z* will be:

`1055Hello5`

# Note

If you add a number and a string, the result will be a string!

---

# JavaScript Logical Operators

| Operator | Description |
| --- | --- |
| && | logical and |
| || | logical or |
| ! | logical not |

# Note

Logical operators are fully described in the **[JS Comparisons](https://www.w3schools.com/js/js_comparisons.asp)** chapter.

---

# JavaScript Type Operators

| Operator | Description |
| --- | --- |
| typeof | Returns the type of a variable |
| instanceof | Returns true if an object is an instance of an object type |

# Note

Type operators are fully described in the **[JS Type Conversion](https://www.w3schools.com/js/js_type_conversion.asp)** chapter.

---

# JavaScript Bitwise Operators

Bit operators work on 32 bits numbers.

Any numeric operand in the operation is converted into a 32 bit number. The result is converted back to a JavaScript number.

| Operator | Description | Example | Same as | Result | Decimal |
| --- | --- | --- | --- | --- | --- |
| & | AND | 5 & 1 | 0101 & 0001 | 0001 | 1 |
| | | OR | 5 | 1 | 0101 | 0001 | 0101 | 5 |
| ~ | NOT | ~ 5 | ~0101 | 1010 | 10 |
| ^ | XOR | 5 ^ 1 | 0101 ^ 0001 | 0100 | 4 |
| << | left shift | 5 << 1 | 0101 << 1 | 1010 | 10 |
| >> | right shift | 5 >> 1 | 0101 >> 1 | 0010 | 2 |
| >>> | unsigned right shift | 5 >>> 1 | 0101 >>> 1 | 0010 | 2 |

The examples above uses 4 bits unsigned examples. But JavaScript uses 32-bit signed numbers.

Because of this, in JavaScript, ~ 5 will not return 10. It will return -6.

~00000000000000000000000000000101 will return 11111111111111111111111111111010

# JavaScript Array Reference

# The JavaScript Array Object

The Array object is used to store multiple values in a single variable.

# Example

const cars = ["Saab", "Volvo", "BMW"];

[Try it Yourself »](https://www.w3schools.com/jsref/tryit.asp?filename=tryjsref_array)

---

# JavaScript Array Methods and Properties

| Name | Description |
| --- | --- |
| https://www.w3schools.com/jsref/jsref_array_at.asp | Returns an indexed element of an array |
| https://www.w3schools.com/jsref/jsref_concat_array.asp | Joins arrays and returns an array with the joined arrays |
| https://www.w3schools.com/jsref/jsref_constructor_array.asp | Returns the function that created the Array object's prototype |
| https://www.w3schools.com/jsref/jsref_copywithin.asp | Copies array elements within the array, to and from specified positions |
| https://www.w3schools.com/jsref/jsref_entries.asp | Returns a key/value pair Array Iteration Object |
| https://www.w3schools.com/jsref/jsref_every.asp | Checks if every element in an array pass a test |
| https://www.w3schools.com/jsref/jsref_fill.asp | Fill the elements in an array with a static value |
| https://www.w3schools.com/jsref/jsref_filter.asp | Creates a new array with every element in an array that pass a test |
| https://www.w3schools.com/jsref/jsref_find.asp | Returns the value of the first element in an array that pass a test |
| https://www.w3schools.com/jsref/jsref_findindex.asp | Returns the index of the first element in an array that pass a test |
| https://www.w3schools.com/jsref/jsref_array_flat.asp | Concatenates sub-array elements |
| https://www.w3schools.com/jsref/jsref_array_flatmap.asp | Maps all array elements and creates a new flat array |
| https://www.w3schools.com/jsref/jsref_foreach.asp | Calls a function for each array element |
| https://www.w3schools.com/jsref/jsref_from.asp | Creates an array from an object |
| https://www.w3schools.com/jsref/jsref_includes_array.asp | Check if an array contains the specified element |
| https://www.w3schools.com/jsref/jsref_indexof_array.asp | Search the array for an element and returns its position |
| https://www.w3schools.com/jsref/jsref_isarray.asp | Checks whether an object is an array |
| https://www.w3schools.com/jsref/jsref_join.asp | Joins all elements of an array into a string |
| https://www.w3schools.com/jsref/jsref_keys.asp | Returns a Array Iteration Object, containing the keys of the original array |
| https://www.w3schools.com/jsref/jsref_lastindexof_array.asp | Search the array for an element, starting at the end, and returns its position |
| https://www.w3schools.com/jsref/jsref_length_array.asp | Sets or returns the number of elements in an array |
| https://www.w3schools.com/jsref/jsref_map.asp | Creates a new array with the result of calling a function for each array element |
| https://www.w3schools.com/jsref/jsref_pop.asp | Removes the last element of an array, and returns that element |
| https://www.w3schools.com/jsref/jsref_prototype_array.asp | Allows you to add properties and methods to an Array object |
| https://www.w3schools.com/jsref/jsref_push.asp | Adds new elements to the end of an array, and returns the new length |
| https://www.w3schools.com/jsref/jsref_reduce.asp | Reduce the values of an array to a single value (going left-to-right) |
| https://www.w3schools.com/jsref/jsref_reduceright.asp | Reduce the values of an array to a single value (going right-to-left) |
| https://www.w3schools.com/jsref/jsref_reverse.asp | Reverses the order of the elements in an array |
| https://www.w3schools.com/jsref/jsref_shift.asp | Removes the first element of an array, and returns that element |
| https://www.w3schools.com/jsref/jsref_slice_array.asp | Selects a part of an array, and returns the new array |
| https://www.w3schools.com/jsref/jsref_some.asp | Checks if any of the elements in an array pass a test |
| https://www.w3schools.com/jsref/jsref_sort.asp | Sorts the elements of an array |
| https://www.w3schools.com/jsref/jsref_splice.asp | Adds/Removes elements from an array |
| https://www.w3schools.com/jsref/jsref_tostring_array.asp | Converts an array to a string, and returns the result |
| https://www.w3schools.com/jsref/jsref_unshift.asp | Adds new elements to the beginning of an array, and returns the new length |
| https://www.w3schools.com/jsref/jsref_valueof_array.asp | Returns the primitive value of an array |

# JavaScript Functions

A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).

# Example

```jsx
// Function to compute the product of p1 and p2function 
myFunction(p1, p2) {  return p1 * p2;}
```

---

# JavaScript Function Syntax

A JavaScript function is defined with the `function` keyword, followed by a **name**, followed by parentheses **()**.

Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).

The parentheses may include parameter names separated by commas:

**(*parameter1, parameter2, ...*)**

The code to be executed, by the function, is placed inside curly brackets: **{}**

function *name*(*parameter1, parameter2, parameter3*) {  // *code to be executed*}

Function **parameters** are listed inside the parentheses () in the function definition.

Function **arguments** are the **values** received by the function when it is invoked.

Inside the function, the arguments (the parameters) behave as local variables.

---

# Function Invocation

The code inside the function will execute when "something" **invokes** (calls) the function:

- When an event occurs (when a user clicks a button)
- When it is invoked (called) from JavaScript code
- Automatically (self invoked)

---

---

# Function Return

When JavaScript reaches a `return` statement, the function will stop executing.

If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.

Functions often compute a **return value**. The return value is "returned" back to the "caller":

# Example

Calculate the product of two numbers, and return the result:

```jsx
// Function is called, the return value will end up in x
let x = myFunction(4, 3);
function myFunction(a, b) {// Function returns the product of a and b  return a * b;}
```

# Why Functions?

With functions you can reuse code

You can write code that can be used many times.

You can use the same code with different arguments, to produce different results.

---

# The () Operator

The () operator invokes (calls) the function:

# Example

Convert Fahrenheit to Celsius:

```jsx
function toCelsius(fahrenheit) {  return (5/9) * (fahrenheit-32);}let value = toCelsius(77);
```

Accessing a function with incorrect parameters can return an incorrect answer:

# Example

```jsx
function toCelsius(fahrenheit) {  return (5/9) * (fahrenheit-32);}let value = toCelsius();
```

Accessing a function without () returns the function and not the function result:

# Example

```jsx
function toCelsius(fahrenheit) {  return (5/9) * (fahrenheit-32);}let value = toCelsius;
```

# Note

As you see from the examples above, `toCelsius` refers to the function object, and `toCelsius()` refers to the function result.

---

# Functions Used as Variable Values

Functions can be used the same way as you use variables, in all types of formulas, assignments, and calculations.

# Example

Instead of using a variable to store the return value of a function:

```jsx
let x = toCelsius(77);let text = "The temperature is " + x + " Celsius";
```

You can use the function directly, as a variable value:

```jsx
let text = "The temperature is " + toCelsius(77) + " Celsius";
```

You will learn a lot more about functions later in this tutorial.

---

# Local Variables

Variables declared within a JavaScript function, become **LOCAL** to the function.

Local variables can only be accessed from within the function.

# Example

```jsx
// code here can NOT use carNamefunction myFunction() {  let carName = "Volvo";  // code here CAN use carName}// code here can NOT use carName
```