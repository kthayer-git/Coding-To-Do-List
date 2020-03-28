# JavaScript Basics

### How Computers Represent our World: (Jon Duckett)
- Computers creates models of the world with data
- Models use Objects to represent physical things
 Objects have:
  - Properties that tell us about the object
  - Methods: perform tasks utilizing the properties of the object
  - Events: triggered when a user interacts with the computer

## Terms and Concepts
- **Expression:** a fragment of code that produces a value

- **Statement:** corresponds to a full sentence, ends with a semi-colon

- **Program:** a list of statements made up of expressions
- **Environment:** the collection of variables and values that exist at a given time

- **Stack** data structure that allows a programmer to push values into it and pop them out in the opposite order, the element that was added last is removed first

- **Object** values that consist of arbitrary collections of properties 

- **Function:** a piece of a program wrapped in a value, a reusable block of code that can accept input  and groups together a sequence of statements to perform a specific task

- **Parameters:** allow functions to accept input(s) and perform a task using the input(s), placeholders for information that will be passed to the function when it is called

- **Default Parameters:** allow parameters to have a predetermined value in case there is no argument passed into the function or if the argument is `undefined `when called

- **Arguments:** values that are passed to the function when it is called

- **Block:** a sequence of statements wrapped in braces

- **Helper Functions:** functions being called within another function using the return value of the first function

- **Function Declaration:** `function` keyword, then name of the function, or its identifier, followed by parentheses and function body, or the block of statements required to perform a specific task, enclosed in the function’s curly brackets, { }

- **Function Expression:** declare a variable to make the variable’s name be the name, or identifier, of your function, common practice to use `const` as the keyword to declare the variable, then assign as that variable’s value an anonymous function created by using the `function` keyword followed by a set of parentheses with possible parameters. Then a set of curly braces that contain the function body

- **String Interpolation:** Using template literals to embed variables into strings

- **Scope:** the part of the program to which the binding is visible

- **Block:** section of code enclosed within curly braces `{}`

- **Block Scope:** scope available to code enclosed by curly braces, allows variables to be defined with precision

- **Local variable:** only available to code that is part of the same block

- **Scope Pollution:** too many variables in the global namespace or reusing variables across different scopes

### Values
- Immutable values: 
  - numbers 
  - strings 
  - Booleans

- Object values (mutable): properties can change, a single object value can have different content at different times

## Methods

 - Methods are actions that can be performed in JavaScript.

 - Properties that hold function values are called **methods** of the value they belong to.
 - Methods are called by appending a JavaScript instance (an object) with a period (dot operator) followed by the name of the method and opening and closing parentheses.
 
- Example:  `'example string'.methodName()`
 - A familiar example:  `console.log()` -calling the `.log() `method on the `console` object.
- Some built-in string properties:
- `.toUpperCase()` - converts all letters to uppercase
- `.toLowerCase()` - converts all letters to lowercase
- `.slice` returns a copy of the string defined by beginning and ending indices, (ending is optional, if no ending is given the rest of the array to end is returned), original string remains unchanged
- `.indexOf` returns the index of the first letter or letters matching the value of the argument(s), if no matching element is found returns -1 , original string remains unchanged
- `.trim` removes whitespace from the start and end of a string
- `.padstart` takes desired and length and padding character as arguments
- `.split` take apart a string with an occurence of another string
- `.join` connect strings
- `.repeat` creates a new string containing multiple copies of the original string joined together 


## Built-in Math Functions
*Examples:*
- `Math.max`
- `Math.min`
- `Math.random`
- `Math.floor`

## Functions Built into Browser
*Examples:*
- `alert();`
- `confirm();`
- `prompt();`


## Control Flow
- Conditional statements: `if` , `else` , `switch`
- Looping statements: `while` , `do` , `for`
- Switch statement: a way to check an expression against multiple values. 

*Example:*
```
const food - 'pizza';
switch(food) {
    case 'oyster':
     console.log('Enjoy the taste of the sea');
     break;
  case 'pizza':
     console.log('Enjoy a delicious pie');
          break;
  default:
     console.log('Enjoy your meal');
}
```

### Bindings and Scope
- `let` and `const` bindings are local to the block in which they were created (post-2015 functions can be built using `let` and `const`)  
- `var` bindings are visible throughout the whole function, or globally if not in a function (pre-2015 JS only functions created new scopes)

### Arrow function with one parameter
- Long version-before applying shortcuts:
`const square1 = (x) => {return x * x; };`
- Shorter version-removing parentheses and brackets:
`const square2 = x => x * x;`

---

## How to use node.js in the terminal:

- type `node-v` and return to get the version of node installed on the computer
- type `node` to enter the node program
- type the javascript commands into terminal and return to see the result. 
Example:
```
> const num = 10;
undefined
> 
> console.log(num);
10
undefined
```
Example:
```
let num1 = 16;
undefined
> console.log(num1);
16
undefined
> console.log(num1 +=1);
17
undefined
> console.log(num1 +=3);
20
```
---
### REPL
- REPL stands for :
  - Read
  - Evaluate
  - Print
  - Loop

### Remainder Operator: `%`
The remainder operator returns the remainder after dividing two numbers. For example, `4 % 2` returns `0`, and `5 % 3` returns `2`.  
The remainder operator is commonly used to find out if a value is even or odd. Even values will have a remainder `0`.

### Quote around Strings in JavaScript
- Ending quote must match beginning quote--both must be the same
- Use straight quotes ( `" "`  or `' '`) not curly quotes
- Always write strings on the same line

### Generating Random Numbers
Use `Math.floor()` and `Math.random()`:
1. Generate a random number between 0 and highest number desired (x):
   ` Math.random() * x;`
2. Since this will produce a decimal, make sure the number is whole using:
    `Math.floor(Math.random() * x);` to round down to the nearest whole number.

### Mathematical Assignment Operators

- `w = w + 1;` is the same as `w += 1;`
- `w = w - 1;` is the same as `w -= 1;`
- `w = w * 1;` is the same as `w *= 1;`
- `w = w / 2;` is the same as `w /= 1;`
- Increment Operator increases the value of the variable by 1:
  - `a = a + 1;` is the same as `a++;`
- Decrement Operator decreases the value of the variable by 1:
  - `b = b - 1;` is the same as `b--;`

### Check Data Type of a Value
`typeof` Operator checks the data type of a value: (this is a Unary Operator as it takes only one value)
```
console.log(typeof b);
// returns number
```

### Logical Operators
- And Operator:
  - `&&` is only true if both values are true (is a Binary Operator)
- Or Operator:
  - `||` is true of either one of the values is true (is also a Binary Operator)
- Not Operator:
  - `!` flips the value given to it (and is a Unary Operator)
- Conditional Operator (also called Ternary Operator)
  - first value ahead of `?` determines whether middle or last value will be returned (is a Ternary Operator)
  - `true ? 1 : 2;`
### Short Circuit Evaluation

*Example:*
- `let defaultName = username || 'Stranger';`

Because `||` or statements check the left-hand condition first, the variable `defaultName` will be assigned the actual value of `username` if is truthy, and it will be assigned the value of `'Stranger'` if `username` is falsy.

### Loop vs. Recursive Function (Eloquent JavaScript)

#### *Loop*

Power function in Eloquent JavaScript using a loop:
```
const power = function (base, exponent) {
    let result = 1;
    for ( let count = 0 ; count < exponent; count++) {
         result *= base;
          }
         return result;
     };
```
#### *Recursive*

Power function in Eloquent Javascript using recursive format:
```
function power (base, exponent) {
     if (exponent == 0) {
        return 1;
      }  else {
        return base * power(base, exponent - 1);
      }
    }
```

## Arrays: Properties and Methods

- `.length` Property that returns the number of items in the array, use dot notation to chain the `.length` property to the array name

- `.push()` Method that adds items to the end of an array, use dot notation to connect to array name, then call it as a function (because it is a built in function) with items to add as arguments, mutates the array by adding elements to it
- `.pop()`Method that removes the last item of an array, use dot notation and connect to array name, removes last element of the array and returns it, takes no arguments, mutates the original array by removing one element
- `.shift()` Method removes the first item from the array and returns the removed element, mutates the array by removing one element
- `.unshift()` Method adds the item in its argument to the beginning of the array, mutates the array by adding one element
- `.slice()` Method returns a copy of the array defined by beginning and ending indices, (ending is optional, if no ending is given the rest of the array to end is returned), original array remains unchanged
- `.indexOf()` Method returns the index of the first element matching the value of the argument, if no matching element is found returns -1 , original array remains unchanged
- `.lastIndexOf()` Method returns the index of last index matching the value of the argument
- `.concat()`  Method used to glue arrays together to create a new array, similar to + for strings

### Array Loop
 - Goes over arrays one element at a time by running the counter over the length of the array:

 *Example:*
```
for (let i = 0; i < array.length; i++ {
      let entry = array[i];
        // perform the computation here
 } 
 ```



### Access Individual Characters in a String (Arrays)

How to access individual characters in a string using bracket notation:
```
const hello = 'Hello World';
console.log(hello[6]);
// Output: W
```

### Ternary Operator

*Example:*

`walkSignal === 'Walk' ? console.log('You may walk!') : console.log('Do not walk!');`