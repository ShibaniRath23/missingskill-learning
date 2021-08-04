# **Array and Object**
# **Array**
* In JavaScript, arrays can be a collection of elements of any type. This means that you can create an array with elements of type String, Boolean, Number, Objects, and even other Arrays.
* An array is a collection of elements or items. Arrays store data as elements and retrieve them back when you need them.
* A pair of square brackets [] represents an array in JavaScript. All the elements in the array are comma(,) separated.

## **Features of array**
* It provides us index which uses numbers to access its 'elements'
* Since arrays are special kind of object it can store different types of variables in the same array.
<br>eg :-
```js
let name = ['push','pull','10','30'];  // Perfectly valid array
```
* Another feature of JS arrays are their built-in properties and methods

## **Array Properties**

| Property | Description |
| ------- | ----------- |
| constructor | Returns the function that created the Array object's prototype |
| length | Returns the number of elements in an array |
| prototype | Allows us to add new properties and method to an array object |


## **Array Methods**

| Methods | Description |
| ------- | ----------- |
| concat | Returns a new array object that contains two or more merged arrays |
| filter | Creates new array with all elements that pass the test in the testing function |
| find | Returns the value of the first element that pass the test in testing function |
| forEach | Calls a function once for each element |
| indexof | Searches the array for an element and return its first index |
| lastIndexOf | Searches the array for an element, starting at the end and returns its last index | 
| isArray | To test if the variable is an array | 
| map | Calls a specified function for every array element and returns a new array | 
| pop | Removes last element from an array | 
| push | Adds a new element to an array | 
| reverse | Reverses the elements of array |
| splice | Adds/Removes element to/from given array |
| slice  | Returns a new array containing the copy of the part of selected array |  
| shift | Removes first element from an array and "shifts" all other elements to lower index |
| unshift | Adds a new element to an array at the start and "unshifts" other elements to higher index |
| toString | Converts an array into string form |

# **Object**

* JavaScript object is a non-primitive data-type that allows you to store multiple collections of data.
```js
// object
const student = {
    firstName: 'gunu',
    class: 5
};
```
Objects can be created in JS using three ways :-
```js
// Using Object Literal
var person = {
  firstName : "Shibani",
  lastName : "Rath",
  age: 23
}

// Using 'new' keyword
var person = new Object();
person.firstName = "Shibani"
person.lastName = "Dhuri";
person.age = "23";

// Using Object Constructor
function Person(fname, lname, age)
{
  this.firstName = fname;
  this.lastName = lname;
  this.age = age;
}
```
## **Object properties**
Properties in object are nothing but the association between names and values. In JS, we can add, delete and modify the properties.

Syntax for accessing prototype :-
```js
objectName.property

// or

objectName['property']

// or

objectName[expression]
```
## **Object Method**

| Methods | Description |
| ------- | ----------- |
| assign | Used to copy properties from source object to target object |
| create | Used to create a new object with specified prototype object and properties |
| keys | Returns an array of given object's own property name |
| values | Returns an array of values |
