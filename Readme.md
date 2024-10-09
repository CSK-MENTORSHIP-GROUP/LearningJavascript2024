# JavaScript Syntax and Basics
## JavaScript Output
- **Writing into an HTML element, using innerHTML. document.write() ,window.alert(),console.log()**
###### innerHTML
```javascript
<!DOCTYPE html>
<html>
<body>
<h2>My First Web Page</h2>
<p>My First Paragraph.</p>
<p id="demo"></p>
<script>
document.getElementById("demo").innerHTML = 5 + 6;
</script>
</body>
</html> 
```
### Statements
```javascript
let x, y, z;    // Statement 1
x = 5;          // Statement 2
y = 6;          // Statement 3
z = x + y;      // Statement 4
```

### JavaScript Syntax

## Comments

## JavaScript Variables
- **let,const,var**

```javascript
let x = 5;
let y = 6;
let z = x + y;
document.getElementById("demo").innerHTML =
"The value of z is: " + z;
```
other variables
```javascript
let person = "John Doe";
let answer = 'Yes I am!';

document.getElementById("demo").innerHTML =
pi + "<br>" + person + "<br>" + answer;
```

### declaring variables
- Always use const if the value should not be changed
- Always use const if the type should not be changed (Arrays and Objects)
- Only use let if you can't use const

### Assignment Operator 
=
==
===

### 
```javascript
let carName = "Volvo";
document.getElementById("demo").innerHTML = carName;
```

### Value = undefined
- A variable declared without a value will have the value undefined.

#### Note
- If you put a number in quotes, the rest of the numbers will be treated as strings, and concatenated.
```javascript
let x = "5" + 2 + 3;
document.getElementById("demo").innerHTML = x;
output: 523
```

```javascript
let x = 2 + 3 + "5";
document.getElementById("demo").innerHTML = x;
// output: 55
```
JS Operators
- Arithmetic Operators
- Assignment Operators
- Comparison Operators
- String Operators
Logical Operators
Bitwise Operators
Ternary Operators
Type Operators

### JavaScript Data Types
String
Number
Bigint
Boolean
Undefined
Null
Symbol
Object
```javascript
// Numbers:
let length = 16;
let weight = 7.5;

// Strings:
let color = "Yellow";
let lastName = "Johnson";

// Booleans
let x = true;
let y = false;

// Object:
const person = {firstName:"John", lastName:"Doe"};

// Array object:
const cars = ["Saab", "Volvo", "BMW"];

// Date object:
const date = new Date("2022-03-25");
```
### JavaScript Functions
- A JavaScript function is a block of code designed to perform a particular task.
- A JavaScript function is executed when "something" invokes it (calls it).

```javascript
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
```

### string methods

```javascript 
let text = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
let length = text.length;
```
## JavaScript if, else, and else if
```javascript
if (hour < 18) {
  greeting = "Good day";
}
``` 

```javascript
const earnings = prompt("enter annual earnings");
const age = prompt("Enter you grade");
if (age < 18 && earnings <= 100000 && (grade == "A" || grade == "B")) {
  console.log("You cant be awarded because you are a kid");
} else if (age >= 18 && earnings > 100000 && (grade == "A" || grade == "B")) {
  console.log("You family earnings decline you eligibility");
} else if (age >= 18 && earnings < 100000 && (grade === "C" || grade === "D")) {
  console.log("You grade disqualifies you");
} else {
  console.log("Disbursement in progress");
}
