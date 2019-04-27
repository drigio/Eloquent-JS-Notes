# Eloquent-JS-Notes

## Chapter One

### Values, Types and Operators

***

#### Basic Types

There are 6 basic types in JS

- Numbers
- Strings
- Booleans
- Undefined
- Null
- Objects

*typeof* Operator

```Javascript
console.log(typeof "Hello World");
// String

console.log(typeof 9.9999);
// Number

console.log(typeof {name: "Adam", age: 23});
// Object
```

#### Type Coercion

When an operator is applied to a *wrong* type of value, Javascript quietly converts it to appropriate type it needs using a set of predefined rules.

```Javascript
console.log("100" + 1);
// 1001

console.log("100" * 1);
// NaN
```

#### Operators

Standard de facto operators found in most of the programming languages 

- **Arithmetic** **(** \- \+ / * %  **)**

- **Logical** **(** && || ! **)**

- **Comparison** **(** > < == != === !== >= <= **)**

#### Short Circuiting of Logical Operators

This concept can be used as a fallback mechanism for default values.

```Javascript
console.log("Adam" || "Eve");
// Adam
console.log(0 || 1);
// 1
console.log("Adam" && "Eve");
// Eve
console.log(0 && 1);
// 0
```

**||** returns the value which is true and comes first.

**&&** returns the value which is false and comes first.

**true || X** - Here X is never evaluated. Once the left hand side of the **||** operator is true, it returns true.

Similarly, **false && X** - will return false without evaluating X

## Chapter Two

### Program Structure

***

Any partial code fragment that returns a value is an **Expression**.

A **Statement** is a declaration that stands on its own and can affect the state of a machine.

The collection of *bindings* and *statements* at a given time is known as an **Environment**.

#### Bindings

Bindings are like tentacles of an octopus, they just hold onto some values not contain them. Two bindings can refer to the same value.

```Javascript
let a = "Something";
console.log(a);
// Something

var b;
console.log(b);
// undefined

const PI = 3.14159
console.log(pi);
// 3.14159

PI = 3.9999 
// TypeError : Reassigning a const binding is not allowed
```

#### Control Flow

Control flow can be changed using any of the following :-
- Conditional Execution
    - if-else
    - switch-case
- Loops
    - while loop
    - do-while loop
    - for loop

#### Comments

```Javascript
// Single Line Comments

/*  This
    is 
    a
    multi-line
    comment
*/
```