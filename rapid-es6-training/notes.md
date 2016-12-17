#Rapid ES6 Training by Mark Zamoyta (from pluralsight.com)

##Introduction

Compatibility with modern broswers: 85-96% (IE to Chrome).

ES6 is backwards compatible with ES5.

New primitive type in ES6: the symbol.
We also have a built-in "promise" object.

kangax.github.io/compat-table/es6 --> this shows browser compatibility for different ES6 features.

##New ES6 Syntax

let: a new keyword used to declare variables. It does away with hoisting. We use *let* to make sure that we _define_ variables before they get used.
var can sometimes result in _closure_ issues (e.g. in a For loop when using "var" to set up "i"). _let_ does away with that problem.

const: stands for constant. We can now declare variables as constants, unable to change.
Constants are defined in UPPERCASE.

Block scoping: when we declare a variable within curly braces, that becomes its scope. We no longer have to rely on function scope. Variables only exist within the block they were defined in.

 