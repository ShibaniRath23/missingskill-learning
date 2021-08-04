# **Introduction to JavaScript**
    JavaScript (js) is a light-weight object-oriented programming language which is used by several websites for scripting the webpages. It is an interpreted programming language that enables dynamic interactivity on websites when applied to an HTML document. It was introduced in the year 1995 by **Brendan Eich**.

## **Versions Of JavaScript**
    
  |Version|Name|
  |-------|-----|
  |ES1- ES2|ECMAScript[1-2](1997)|
  |ES3|ECMAScript 3(1999)|
  |ES5|ECMAScript 5(2009)|
  |ES6|ECMAScript 6(2015)|


> JavaScript  is also known as ECMAScript.

## **JavaScript Variables**

   * Variables are containers for storing data (values).

    In this example, x, y, and z, are variables, declared with the var keyword:

```js
Example
    var x = 5;
    var y = 6;
    var z = x + y; 
    
```
  Output
  The value of z is: 11

## **JavaScript Data Types**

     There are two types of data type in JavaScript.
  1. Primitive data type
  2. Non-Primitive data type

### 1. Primitive data type:
       1. String
       2. Number
       3. Boolean
       4. Undefined
       5. Null
       6. Sysmbol( ES6)
    > type of (Null) is object and treated as falsy for boolean operations.
    > type of (Undefined) is Undefined and treated as falsy for boolean operations.

### 2. Non-Primitive data type:
       1. Array []
       2. Object {}
   
   > Examples:
 ```js
      Roll = 20;                                      // Number
      Name = "Shibani";                               // String
      x = {firstName:"Banaja", lastName:"Mishra"};    // Object

  ```
## **JavaScript keywords**
    *  keywords are  reserve words which has some special meaning and uesd to declare variables.
       1. var  (ES5)
       2. let  (ES6)
       3. const(ES6)

### **Differnce between Var,let and const :**
     
  |var |let|const|
  |----|----|---|
  |ES5|ES6|ES6|
  |Can be redeclared.|can not be redeclared.|can not be redeclared.|
  |Functional/Global scope|lexcical/Block scope|lexcical/Block scope|
  |Can be reinitialised.|Can be reinitialised.|Can not be reinitialised.|
  |Can be hoisted.|Can not be hoisted.|Can not be hoisted.|

## **JavaScript Operator**
      JavaScript operators are symbols that are used to perform operations on operands.
### **Types of Operator**
    1. Arithmetic Operator
    2. Comparison (Relational) Operator
    3. Bitwise Operator
    4. Logical Operator
    5. Assignment Operator
    6. Ternary Operator

### 1.Arithmetic Operators:

|Operator|Description|Example|
|-------|-----------|--------|
|+	|Addition|10+20=30|
|-	|Subtraction|20-19=1|
|*	|Multiplication|3*5=15|
|**	|Exponentiation|2**3=8|
|/	|Division|200/10=20|
|%	|Modulus (Division Remainder)|200%10=0|
|++	|Increment|var a=10; a++; Now a = 11|
|--	|Decrement|var a=10; a--; Now a = 9|

### 2.Comparison (Relational) Operators:

|Operator|	Description	|Example|
|-------|---------------|-------|
|==|	Is equal to|	10==20 = false|
|===|	Identical (equal and of same type)|	10==20 = false|
|!=	|Not equal to|	10!=20 = true|
|!==|Not Identical|	20!==20 = false|
|>|	Greater than|	20>10 = true|
|>=|	Greater than or equal to|	20>=10 = true|
|<|	Less than	|20<10 = false|
|<=	|Less than or equal to	|20<=10 = false|

### 3.Bitwise Operator:

|Operator|	Description	|Example|
|--------|--------------|-------|
|&	|Bitwise AND|	(10==20 & 20==33) = false|
||	|Bitwise OR	|(10==20 | 20==33) = false|
|^	|Bitwise XOR|	(10==20 ^ 20==33) = false|
|~|	Bitwise NOT|	(~10) = -10|
|<<|	Bitwise Left Shift	|(10<<2) = 40|
|>>|	Bitwise Right Shift	|(10>>2) = 2|

### 4.Logical Operator:

|Operator|	Description	|Example|
|--------|-------------|--------|
| && |Logical AND|(10==20 && 20==33) = false|
| !  |Logical Not|!(10==20) = true|

###  5.Assignment Operator

|Operator|	Description	|Example|
|--------|--------------|------|
|=|	Assign	|10+10 = 20|
|+=|	Add and assign|	var a=10; a+=20; Now a = 30|
|-=|	Subtract and assign	|var a=20; a-=10; Now a = 10|
|/=|	Divide and assign|	var a=10; a/=2; Now a = 5|
|%=|	Modulus and assign|	var a=10; a%=2; Now a = 0|
 
 >### **Values for boolean operations:** 

      * Falsy value:(false) zero ,undefined, "",Null,NaN.
      * Truthy value:(true) object, array
  
### 6.Ternary Operator:
    (?:)	Conditional Operator returns value based on the condition. It is like if-else.

## **JavaScript Control Structure**
 
     1. If else
     2. for loop
     3. switch case
     4. while loop
     5. do ... while

## **Scope in JavaScript:**
 
    In the JavaScript language there are two types of scopes:

    I. Functional Scope
       1.Global Scope
       2.Local Scope
    II. Lexical Scope

   Variables defined inside a function are in local scope while variables defined outside of a function are in the global scope. Each function when invoked creates a new scope.

 **Functional Scope** : Each program or application  can be called as functional scope(global functional scope). And each function within program  have their own functinal scope(local functional scope) which exist untill the function exists. `var` keyword has functional scope.

### 1.Global Scope:
  A variable is in the Global scope if it's defined outside of a function.Variables inside the Global scope can be accessed and altered in any other scope.


### 2.Local Scope:
  Variables declared within a JavaScript function, become LOCAL to the function.
   local variables defined within functions,can only be used within that function in which they are defined its scope exist only within that function not outside of that function.

```js
example:
 var a;
 var b ="ok";
 Console.log(a+b);
 a=20;

 function hello()
 {
   console.log(a);
 }
 hello();
 a=10;

 ```
**Lexical Scope/Block Scope** : starts and end with curly braces `{ }`also called block is lexical scope/block scope. Any variable that exist only inside curly braces `{ }` has lexical scope.`let` and `const` have lexical scope.
```js
 let a=4;
 if(a){
   let b=9;
   let a=9;
   console.log(a+b);
   b=a+b;
 }
 ```
 ```js
 output:18
 ```
## Tech Debt

### 1.Concat & Addition:

JavaScript uses '+' operator for both addition and concatenation. Simply put numbers will be added and Strings will be concatenated. JS interpreter works from left to right.

```js
var x = 10;
var y = 10;
var z = "10";

var result = x + y + z; // Result will be 2010  
```
### 2.NaN:

`NaN` is a reserved keyword to indicate that number is not legal number.

Eg :-
```js
var x = 100/"Apple"; // x will be NaN
```
## **Copy by Value & Copy by Reference**
### **Copy by Value**:
   * In Copy by value, function is called by directly passing the value of the variable as an       argument.So any changes made inside the function does not affect the original value.
  Primitive datatype  follows  copy by value property.

```js
function square(x) {
    x = x * x;
    return x;
}
var y = 10;
var result = square(y);
console.log(y); // 10 -- no change
console.log(result); // 100 
```
### **Copy by Reference**:
   * In copy by Reference, Function is called by directly passing the reference/address of the variable as an argument. So changing the value inside the function also change the original value. In JavaScript array and Object follows copy by reference property.
```js
var stack={
   node:100,
   php=200,
   go=300,
   es:[5,6,8,9,10]
}

console.log("1", stack);//{node:100,php:200,go:300,es:[5,6,8,9,10]}
var tech=stack;
tech.go=10;
console.log("2",stack.go);//10










     





    

