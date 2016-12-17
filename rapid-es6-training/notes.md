#Rapid ES6 Training by Mark Zamoyta (from pluralsight.com)

##Introduction

Compatibility with modern broswers: 85-96% (IE to Chrome).

ES6 is backwards compatible with ES5.

New primitive type in ES6: the symbol.
We also have a built-in "promise" object.

kangax.github.io/compat-table/es6 --> this shows browser compatibility for different ES6 features.

##New ES6 Syntax

###let
A new keyword used to declare variables. It does away with hoisting. We use *let* to make sure that we _define_ variables before they get used.
var can sometimes result in _closure_ issues (e.g. in a For loop when using "var" to set up "i"). _let_ does away with that problem.

###const
Stands for constant. We can now declare variables as constants, unable to change.
Constants are defined in UPPERCASE.

###Block scoping
When we declare a variable within curly braces, that becomes its scope. We no longer have to rely on function scope. Variables only exist within the block they were defined in.

###Arrow Functions, =>
The symbol is called "fat arrow". It's a shorthand notation that allows us to leave out the keywords "function" and "return". Examples:

```
 var getPrice = () => 5.99;
 console.log(typeof getPrice); // function
```
```
 var getPrice = () => 5.99;
 console.log(getPrice()); // 5.99
```
```
 var getPrice = count => count * 4.00;
 console.log(getPrice(2)); // 8
```
```
 var getPrice = (count, tax) => count * 4.00 * (1 + tax);
 console.log(getPrice(2, .07)); // 8.56
```

 The _return_ keyword does need to be used if the function contains a block rather than a one-line return statement.

 The main purpose of arrow functions is to handle the _this_ keyword within functions. Arrow functions are intended to de-mystify the _this_ keyword in functions.

 In ES5, _this_ gets set to the element that's receiving the event. In ES6, _this_ gets set to the context of the code we're in.

 The fat arrow symbol can't be placed on a new line. It has to be in-line with the beginning of the function.

 We don't have access to a prototype field when declaring a function with the fat arrow symbol.