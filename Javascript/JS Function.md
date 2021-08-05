# **JavaScript Functions**
* A function is a block of code that performs a specific task.
## **Benefits of Function**
* Function makes the code reusable. You can declare it once and use it multiple times.
* Function makes the program easier as each small task is divided into a function.
* Function increases readable.
## **Properties of a function**
* can be an object.
* can be value in array.
* Can be `assigned to variable`.
* Can also `return another function` , if no variable or value is returned from function it returns `undefined`.
* Can be `pass as parameter`, if we don't pass argument while calling a parameterized function then by default is `undefined`.

## **Declaring a Function**
* A function is declared using the function keyword.
* The basic rules of naming a function are similar to naming a variable. It is better to write a   descriptive name for your function. For example, if a function is used to add two numbers, you could name the function add or addNumbers.
* The body of function is written within {}.
  The syntax to declare a function is:
```js
function nameOfFunction () {
    // function body   
}
```
## **Function call & Declaration**
```js
// declaring a function
function wave() {
    console.log("Hello there!");
}

// calling the function
wave();
```
## **Function Parameters**
* A function can also be declared with parameters. A parameter is a value that is passed when declaring a function.
```js
// declaring a function
function add(a, b) {
    console.log(a + b);
}

// calling functions
add(3,4);
add(2,9);

output:
7
11
```
## **Function Return**
The return statement can be used to return the value to a function call.

```js
 function hello(some value)
 {
     console.log("print"+some value);
     return some value * 2;
 }
 var val=20;
 var result=hello(val);
 console.log(result);

 output:
 print 20
 40
```
## **Higher order function(concept) :**
function takes function as parameter and return function.
## **Pure function**
* Pure functions always returns the same result if the same arguments are passed in.
```js
function add(a,b){
    return a+b;
}
var x=20;
var y=30;
const result=add(x,y);
console.log(result);

output:50
```
## **Arrow function**
* Arrow functions, introduced in ES6, provides a concise way to write functions in JavaScript.
```js
let add = (x, y) => x + y;

console.log(add(10, 20)); // 30;
```
_NORMAL FUNCTION_
```js
   let add = function (x, y) {
	return x + y;
   };

console.log(add(10, 20)); // 30
```

## **IIFE**( Self Excuting Function)
* An Immediately-invoked Function Expression (IIFE) is a way to execute functions immediately, as soon as they are created.
Syntax :
```js
(function() {
  /* */
})();
```
Example:
```js
(function() {
  console.log("self excuting function");
})();
```
## **Inline Function**
It is a function that is integrated directly into the calling code. It helps to optimize code .
Example :
```js
let email = (function(greet){
    
    function body(name){
        let final = !!greet && (typeof greet === 'function') && greet(name);  
        return final;
    }

    return body;
})(function(name){               //inline function, anonymous function
    return `Hi, ${name}`; 
});

let person1 = email('mishra');
console.log(person1); //Hi, mishra
```
## **JavaScript Constructor & Prototype**
* A constructor is a function that creates an instance of a class which is typically called an “object” In JavaScript, a constructor gets called when you declare an object using the new keyword.
```js
function User(first, last) {
  this.firstName = first
  this.lastName = last
}
var user1 = new User("BANAJA", "MISHRA")
console.log(user1)
var user2 = new User("LITAN", "KAR")
console.log(user2)

output:
User { firstName: 'BANAJA', lastName: 'MISHRA' }
User { firstName: 'LITAN', lastName: 'KAR' }
```

## **Prototypes**

- Array
- Object
- Function
- String
- Boolean
- Number
- RegExp
- Date
- Math


 
**Date**

* It returns the date like day, month, year.
   ex:  getDate(), getHours(), getMonth(),getMinutes() etc.

**Math**

* It is used for mathematical operation.
   ex:  random(), floor(), max(), min(), sqrt(),etc.







