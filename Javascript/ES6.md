# **ES6**

## **BUILT-IN-FUNCTION IN ES6** 
ES6 is also known as ECMAScript 6. ES6 version brought lots of new syntax and new features that makes our code more modern and more readable. Essentially it helps us write less code and do more.

|Functions|Used For|Syntax|
|---------|--------|------|
|SetTimeOut|The code will run after some time.|setTimeout(param1,time)|
|SetInterval|It will execute in continous loop.|setInterval(param1,time)|
|ParseInt|It converts any thing into integer number.|parseInt(param)|
|ParseFloat|It parse through string and return float value.|parseFloat(param)|
|JSON|JSON is often used to send data overnetwork.|{"key":"Value"}|

## **JSON**
 
- It stands for Javascript object notation.
- It can be used for transfer and recieve data from one application to another application.
- It contains data in terms of key value pair.
- JSON data are always stored in double Qoute " ".
- It has two method for transfer and recieve data 
     -  JSON.stringify(obj)
     -  JSON.Parse(Obj);

example
```js
        const send_data = JSON.stringify(x);// Used for sending data

        const recieve_data = JSON.parse(send_data);// use for receiving data
```

## **Template Literals**
 * Template literals are string literals allowing embedded expressions using {`${}`}.
   Ex:

```JS
var firstName = "Shibani";
var lastName = "Rath";
console.log(`${firstName} ${lastName}`);
```
## **Destructuring**
*  It is used to assign elements of array/object into variable</b>

```Js
// Array destructuring
var name = ["sam", "mike", "doe"];

var [first, second, third] = name;

// Object destructuring
var user = {
  id = 1,
  name = "Mike",
}

var {id,name} = user;
```
## **Spread Operator**
 * It is used with three dots(...) which targets the entire values in the particular variable.

```Js
let colors = ['Red', 'Yellow'];  
let newColors = [...colors, 'Violet', 'Orange', 'Green'];  
console.log(newColors);  
```
## **Rest Operator**
 * It is also same as Spread operator that can be used in destructuring.

```Js
var colors = [ "Blue", "Green", "Yellow",  "Red"];    
    
// destructuring assignment    
var [a,b,...args] = colors;  
```





