# Function Types

## Learning Goals

- Return Types
- Parameter Types
- Function Documenting

## Introduction

Whether created locally in a file, imported from another file, or even as a
method on a class, functions are the basic building blocks in all JavaScript
applications. Using TypeScript with our functions takes them to the next level
by not only making them easier to work with, but by giving them even more
capabilities!

## Return Types

By assigning a type to our return, we are able to ensure that our functions will
always return what we expect. Let's create a simple `sum` function,
that takes two numbers in as arguments and returns their sum.

```ts
function sum(num1, num2){
 return num1 + num2
}

// Nice! This seems like a pretty straight forward, non-error-prone function,
// right? Let's test it out!

sum(2,3)
// => 5 
// Perfect!

sum(2, '3')
// => '23'
// .... Wait, what?!
```

Ah yes, the classic javascript return blunder! Let's annotate a return type to
fix this incredibly common and annoying bug.

```ts
function sum(num1, num2): number{
 return num1 + num2
}
```

By running our compiler, we immediately get a very clear and helpful error:

```ts
index.ts: - error TS2345: Argument of type 'string' is not assignable to parameter of type 'number'.

12 sum(2, '3')
          ~~~
```

Nice! TypeScript can often assume our assume our return types, but for clarity
and the sake of documentation, annotating a functions return type is a great
habit to get into. Let's look at some of the ways we can use TypeScript to shape
our returns.

### implicit return

- implicit return

### explicit return

- explicit return

### void return

- void return

## Parameter Type Annotations

- this is how we add param types

### Optional Parameters

- this is an optional parameter

### Default Parameters

- this is a default parameter



## Documenting Functions

- why we document functions
- how we document functions

## Conclusion

in this lesson we covered:

- Parameter Types
- Return Types
- Function Documenting

## Resources

- [Return Type Annotations](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#return-type-annotations)
- [link 2]('')
