<b> Q1. What are the basic data types in TypeScript?</b>

Data types in TypeScript are of 2 types:

<li>Built-in data type or primitive data type</li>
<li>User defined data type</li>

<br>
<b>Built-in or primitive data type:</b>

1. <b>Number</b> : These numeric values are treated like a number data type. The numeric data type can be used to represents both integers and fractions. TypeScript also supports Binary(Base 2), Octal(Base 8), Decimal(Base 10), and Hexadecimal(Base 16) literals.

    <b>Syntax :</b>
    
    ```
    let identifier: number = value;
    ```
2. <b>String : </b>  We will use the string data type to represents the text in TypeScript. String type work with textual data. We include string literals in our scripts by enclosing them in single or double quotation marks. It also represents a sequence of Unicode characters.   

    <b>Syntax : </b>
    ```
        let identifier: string = " ";  
                    Or   
        let identifier: string = ' ';  
    ```

 3. <b>Boolean : </b> The Boolean data type can have only two values. They are "true" and "false." A Boolean value is a truth value which specifies whether the condition is true or not.

    <b>Syntax : </b>
    ```
    let identifier: BooleanBoolean = Boolean value;  
    ```

4. <b>Void : </b> A void is a return type of the functions which do not return any type of value. It is used where no data type is available. A variable of type void is not useful because we can only assign undefined or null to them.

   <b>Syntax : </b>
   ```
   let unusable: void = undefined;  
   ```  

5. <b>Null : </b>  Null represents a variable whose value is undefined.  
<br>
6. <b>Undefined : </b>The Undefined primitive type denotes all uninitialized variables in TypeScript and JavaScript. It has only one value, which is undefined. The undefined keyword defines the undefined type in TypeScript, but it is not useful because we can only assign an undefined value to it.

<b>User defined data types : </b>

1. <b>Array : </b> An array is a collection of elements of the same data type. Like JavaScript, TypeScript also allows us to work with arrays of values. An array can be written in two ways:

   ```
   var list : number[] = [1, 3, 5];  
   ```
   ```
   var list : Array<number> = [1, 3, 5];  
   ```

2. <b>Touple : </b> The Tuple is a data type which includes two sets of values of different data types. It allows us to express an array where the type of a fixed number of elements is known, but they are not the same. For example, if we want to represent a value as a pair of a number and a string, then it can be written as:
    ```
   // Declare a tuple  
      let a: [string, number];  
  
    // Initialize it  
      a = ["hi", 8, "how", 5]; // OK  
    ```

3. <b>Enums : </b> Enums define a set of named constant. TypeScript provides both string-based and numeric-based enums. By default, enums begin numbering their elements starting from 0, but we can also change this by manually setting the value to one of its elements. 

<br>
<b>Q2. What is Generic data type.</b>

<br>

In TypeScript, Generics are basically a kind of tool that enables you to create reusable code components that work with a number of types instead of a single type.

In generics, we pass a parameter called type parameter which is put in between the lesser sign (<) and the greater sign (>), for example, it should be like <type_parameter_name>.

<b>Syntax : </b>
```
  function function_name <type_parameter> 
    (parameter_name : data_type_parameter) 
    : return_type_parameter {
        // Rest code......
    }
```

<b>Q3. What is type inferring in TS?</b>

TypeScript infers types of variables when there is no explicit information available in the form of type annotations.

Type inference is helpful in type-checking when there are no explicit type annotation is available. In type inference, there can be a situation where an object may be initialized with multiple types.

<b>Q4. What are the possible ways to define typing for functions.</b>

In TypeScript, there are multiple syntaxes for declaring the type of a function:

<li>Method signatures</li>
<li>Function type literals</li>
<li>Object type literals with call/construct signatures</li>
<br>
<b>Method Signatures : </b>
The method signature syntax is probably the most straightforward to use. When defining an object type, its methods can easily be described by providing signatures as follows:


```
interface Date {
  toString(): string;
  setTime(time: number): number;
  // ...
}
```

<b>Function Type Literals : </b>
Function type literals are another way to declare the type of a function. They're typically used in the signature of a higher-order function, that is, a function which accepts functions as parameters or which returns a function:
```
interface Array<T> {
  sort(compareFn?: (a: T, b: T) => number): this;
  // ...
}
```
<b>Object Type Literals with Call or Construct Signatures : </b>
In JavaScript, functions are nothing but special objects than can be called. This fact is reflected in the syntax of object type literals: they describe the shape of an object, which also happens to have a call signature:

```
interface RegExpConstructor {
  // Call signatures
  (pattern: RegExp): RegExp;
  (pattern: string, flags?: string): RegExp;

  // ...
}
```

<b>Q5. How to define Generic type for classes. </b>

TypeScript also supports generic classes. The generic type parameter is specified in angle brackets (<>) following the name of the class. A generic class can have generic fields or methods.

<b>Example : </b>
```
class GenericNumber<NumType> {
  zeroValue: NumType;
  add: (x: NumType, y: NumType) => NumType;
}
 
let myGenericNumber = new GenericNumber<number>();
myGenericNumber.zeroValue = 0;
myGenericNumber.add = function (x, y) {
  return x + y;
};
```