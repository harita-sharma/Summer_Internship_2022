<b>Q1. What are anonymous functions in javascript?</b>

 In JavaScript, an anonymous function is that type of function that has no name or we can say which is without any name. When we create an anonymous function, it is declared without any identifier.Anonymous functions are created using the function operator.

<b>Example-</b>
```
let demo = function (){

console.log("Example of anonymous functions");

}

demo();
```


<br>

<b> Q2. Explain strict comparison and Abstract comparison in javascript?</b>

<b>Abstract Equality Operator (==):</b>

The Abstract Equality Operator checks whether two operands are equal and returns true if equal, false otherwise.Also known as loose equality.This operator compares if two values look similar.

<b>Example:</b>
```
console.log(3 == "3"); // true
```

<b>Strict Equality Operator (===):</b>

The Strict Equality Operator checks whether two operands are equal and are of the same type.If the values have different types, the values are considered unequal. If the values have the same type, are not numbers, and have the same value, they're considered equal.

<b>Example:</b>
```
console.log(3 === "3"); // false.
```

Using two equal signs returns true because the string “3” is converted to the number 3 before the comparison is made. Three equal signs sees that the types are different and returns false.

<br>

<b> Q3. Difference between arrow functions and regular functions?</b>

<b>Regular function:</b>
Regular functions created using function declarations or expressions are constructible and callable.Since regular functions are constructible, they can be called using the new keyword.

<b>Syntax</b>
```
let x = function function_name(parameters){

   // body of the function

};
```
<b>Example of regular functions:-</b>
```
let square = function(x){

  return (x*x);

};

console.log(square(9));
```
<b>
Output: 81
</b>

<br>

<b>
Arrow function:</b>

Arrow functions are only callable and not constructible, i.e arrow functions can never be used as constructor functions. Hence, they can never be invoked with the new keyword. 

<b>Syntax</b>

```
let x = (parameters) => {

    // body of the function
    };
```

<b>Example of arrow functions:-</b>

```
var square = (x) => {

return (x*x);

};

console.log(square(9));
```

<b>
Output: 81
</b>

<br>

If a function is constructable, it can be called with new, i.e. new User(). If a function is callable, it can be called without new (i.e. normal function call).

<br>

<b> Q4. What is Hoisting in javascript?</b>

Hoisting in JavaScript is a behavior in which a function or a variable can be used before declaration.

The JavaScript compiler moves all the declarations of variables and functions at the top so that there will not be any error. This is called hoisting.


 <b>Declaration -> 2.Initialisation/Assignment ->3. Usage</b>

<br>
 

 <b>Q5. Javascript is a garbage collected programming language, explain how? </b>

 JavaScript is a unique language. Unlike other languages, JavaScript is able to automatically allocate memory when it is needed. It can also release that memory when it is not needed anymore.
 
 The main concept garbage collection relies on is the concept of references and reachability. It distinguishes between values that are reachable and values that are not. Values that are reachable are local variables and parameters in a current function. If there are nested functions in the chain, reachable values are also parameters and variables of these nested functions.
 
 One thing programming languages share is something called memory life cycle.

<li>The first step is about allocating the memory you need.</li>

<li>The second step is about using that allocated memory for tasks such as read and writing data.</li>

<li>The third and final step is about releasing that allocated memory.</li>

JavaScript takes care of memory management for you. It automatically handles all those three steps of memory life cycle.

<br>

<b>Q6. Explain Shallow vs Deep copy in JS?</b>

<b>Deep copy:</b>
A deep copy means that all of the values of the new variable are copied and disconnected from the original variable. 

deep copy makes a copy of all attributes of the old object and allocates separate memory addresses for the new object.

<b>Shallow copy:</b>
 A shallow copy means that certain (sub-)values are still connected to the original variable. 
 
 Basically, if any of the fields of the objects are referenced to other objects they share the same memory address.

 <br>

 <b>Q7. What is Object.freeze? </b>

 The Object.freeze() method freezes an object. A frozen object can no longer be changed; freezing an object prevents new properties from being added to it, existing properties from being removed, prevents changing the enumerability, configurability, or writability of existing properties, and prevents the values of existing properties from being changed. In addition, freezing an object also prevents its prototype from being changed. freeze() returns the same object that was passed in.

 <b>Syntax</b>

 ```
 Object.freeze(obj)
 ```

<b>Program-</b>

<b>Q1. Write a function that generate a random number between two range, -100 to 0 and 800-900.</b>

```
 function randomNumber(min, max){

return Math.random(Math.random()*(max-min+1) + min)
}

const rndNum1=randomNumber(-100, 0);

const rndNum1=randomNumber(800, 900);

console.log(rndNum1);

console.log(rndNum2);
```

<b>Output:

 -48

876</b>
