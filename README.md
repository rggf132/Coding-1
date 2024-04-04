# Coding-1

## Setup 

1. Make GitHub account (Best via Google)
2. Download [GitHub Windows Application](https://desktop.github.com/)
3. Clone this Repository via GitHub Application to Computer.
4. Install [NodeJs](https://nodejs.org/en/download)
5. Open `cmd` and typing `node` should run the command without errors.

## Data Types in JavaScript

In JavaScript, types refer to the various data types that variables and values can have. Here are the primary data types in JavaScript:

### Primitive Types
- **String**: Represents textual data, enclosed within single (`' '`), double (`" "`), or backtick (\` \`) quotes.
- **Number**: Represents numeric data, including integers and floating-point numbers. JavaScript doesn't differentiate between integers and floats.
- **Boolean**: Represents a logical entity and can have two values: `true` or `false`.
- **Undefined**: Represents a variable that has been declared but has not been assigned a value.
- **Null**: Represents the intentional absence of any object value.
- **Symbol**: Represents a unique identifier, introduced in ECMAScript 6 (ES6).

### Non-primitive Types (Reference Types)
- **Object**: Represents a collection of key-value pairs. Objects can be created using object literals `{}`, constructor functions, or classes.
- **Array**: Represents a special type of object used to store multiple values in a single variable. Arrays can hold any data type, including other arrays (nested arrays).
- **Function**: Represents a reusable block of code that can be called with a set of parameters.
- **Date**: Represents a date and time value.
- **RegExp (Regular Expression)**: Represents a sequence of characters that defines a search pattern.

JavaScript is a dynamically typed language, meaning you don't have to explicitly specify the data type of a variable when declaring it. JavaScript determines the data type of a variable automatically based on the value assigned to it. Additionally, JavaScript is loosely typed, meaning variables can change types as needed during runtime.


## Examples of JavaScript Data Types

### Primitive Types

#### String
```javascript
let str = 'Hello, world!';
```

#### Number
```javascript
let num = 42;
```

#### Boolean
```javascript
let isTrue = true;
let isFalse = false;
```

#### Undefined
```javascript
let undefinedVar;
```

#### Null
```javascript
let nullVar = null;
```

#### Symbol
```javascript
const sym = Symbol('description');
```

### Non-primitive Types (Reference Types)

#### Object
```javascript
let person = {
  name: 'John Doe',
  age: 30
};
```

#### Array
```javascript
let fruits = ['apple', 'banana', 'orange'];
```

#### Function
```javascript
function greet(name) {
  console.log('Hello, ' + name + '!');
}

greet('Alice'); // Output: Hello, Alice!
```

#### Date
```javascript
let currentDate = new Date();
```

#### RegExp (Regular Expression)
```javascript
let regex = /[a-zA-Z]+/;
```

## Excercises - Primitives

### String

1. **Concatenation**: Create a string variable containing your first name and another string variable containing your last name. Then, concatenate them together and print the result.
   
   ```javascript
   let firstName = 'John';
   let lastName = 'Doe';
   let fullName = firstName + ' ' + lastName;
   console.log(fullName); // Output: John Doe
   ```

2. **String Length**: Declare a string variable and find out its length using the `length` property.
   
   ```javascript
   let str = 'Hello, world!';
   console.log(str.length); // Output: 13
   ```

3. **Substring**: Given a string, extract a substring from it using the `substring` method.
   
   ```javascript
   let str = 'JavaScript is awesome!';
   let substr = str.substring(0, 10); // Extracts characters from index 0 to 9
   console.log(substr); // Output: JavaScript
   ```

### Number

1. **Arithmetic Operations**: Perform basic arithmetic operations (addition, subtraction, multiplication, division) on two number variables.
   
   ```javascript
   let num1 = 10;
   let num2 = 5;
   console.log(num1 + num2); // Output: 15
   console.log(num1 - num2); // Output: 5
   console.log(num1 * num2); // Output: 50
   console.log(num1 / num2); // Output: 2
   ```

2. **Increment and Decrement**: Increment and decrement a number variable by one.
   
   ```javascript
   let num = 10;
   num++; // Increment by one
   console.log(num); // Output: 11
   num--; // Decrement by one
   console.log(num); // Output: 10
   ```

3. **Modulus Operator**: Use the modulus operator to find the remainder of division between two numbers.
   
   ```javascript
   let num1 = 10;
   let num2 = 3;
   console.log(num1 % num2); // Output: 1 (Remainder of 10 divided by 3)
   ```

### Boolean

1. **Logical Operations**: Perform logical operations (AND, OR, NOT) between two boolean values.
   
   ```javascript
   let isSunny = true;
   let isRainy = false;
   console.log(isSunny && isRainy); // Output: false (AND operation)
   console.log(isSunny || isRainy); // Output: true (OR operation)
   console.log(!isRainy); // Output: true (NOT operation)
   ```

2. **Comparison Operators**: Use comparison operators to compare two numbers and two strings.
   
   ```javascript
   let num1 = 10;
   let num2 = 5;
   console.log(num1 > num2); // Output: true
   console.log(num1 === num2); // Output: false
   
   let str1 = 'apple';
   let str2 = 'banana';
   console.log(str1 !== str2); // Output: true
   ```

3. **Conditional Statements**: Write a conditional statement using boolean values to control program flow.
   
   ```javascript
   let isLogged = true;
   if (isLogged) {
       console.log('User is logged in.');
   } else {
       console.log('User is not logged in.');
   }
   ```

## Excercises - Non Primitives

### Object

1. **Accessing Object Properties**: Create an object representing a person with properties such as name, age, and occupation. Then, access and print individual properties.
   
   ```javascript
   let person = {
     name: 'John Doe',
     age: 30,
     occupation: 'Engineer'
   };
   console.log(person.name); // Output: John Doe
   console.log(person.age); // Output: 30
   console.log(person.occupation); // Output: Engineer
   ```

2. **Adding and Modifying Properties**: Add a new property to an existing object and modify an existing property.
   
   ```javascript
   let car = {
     make: 'Toyota',
     model: 'Camry',
     year: 2018
   };
   car.color = 'blue'; // Add new property
   car.year = 2020; // Modify existing property
   console.log(car); // Output: { make: 'Toyota', model: 'Camry', year: 2020, color: 'blue' }
   ```

3. **Object Methods**: Create an object representing a calculator with methods for addition, subtraction, multiplication, and division.
   
   ```javascript
   let calculator = {
     add: function(num1, num2) {
       return num1 + num2;
     },
     subtract: function(num1, num2) {
       return num1 - num2;
     },
     multiply: function(num1, num2) {
       return num1 * num2;
     },
     divide: function(num1, num2) {
       return num1 / num2;
     }
   };
   console.log(calculator.add(5, 3)); // Output: 8
   console.log(calculator.multiply(2, 4)); // Output: 8
   ```

### Array

1. **Accessing Array Elements**: Create an array of fruits and access individual elements by index.
   
   ```javascript
   let fruits = ['apple', 'banana', 'orange'];
   console.log(fruits[0]); // Output: apple
   console.log(fruits[1]); // Output: banana
   console.log(fruits[2]); // Output: orange
   ```

2. **Array Length**: Determine the length of an array using the `length` property.
   
   ```javascript
   let colors = ['red', 'green', 'blue'];
   console.log(colors.length); // Output: 3
   ```

3. **Array Methods**: Use array methods such as `push`, `pop`, `shift`, and `unshift` to modify arrays.
   
   ```javascript
   let numbers = [1, 2, 3];
   numbers.push(4); // Add an element to the end
   numbers.pop(); // Remove the last element
   numbers.unshift(0); // Add an element to the beginning
   numbers.shift(); // Remove the first element
   console.log(numbers); // Output: [2, 3, 4]
   ```

### Function

1. **Function Declaration**: Declare a function that takes two parameters and returns their sum.
   
   ```javascript
   function addNumbers(num1, num2) {
     return num1 + num2;
   }
   console.log(addNumbers(5, 3)); // Output: 8
   ```

2. **Function Expression**: Assign a function to a variable and then call it.
   
   ```javascript
   let greet = function(name) {
     console.log('Hello, ' + name + '!');
   };
   greet('Alice'); // Output: Hello, Alice!
   ```

3. **Arrow Function**: Use an arrow function to calculate the square of a number.
   
   ```javascript
   let square = num => num * num;
   console.log(square(4)); // Output: 16
   ```
