[Home](https://zx37.github.io/learning-journal/)

# Operators and Loops

## Comparative operators:

The following operators are used to compare two values in JavaScript. Comparisons are commonly used in `for` and `while` loops and return a boolean true or false value.

- `==` - is equal to
- `===` - is equal to (strict typing)
- `!=` - is not equal to
- `!==` - is not equal to (strict typing)
- `>` - is greater than
- `>=` - is greater than or equal to
- `<` - is less than
- `<=` - is less than or equal to

Multiple comparisons can be combined using the following logical operators to create more complex conditionals.

- `&&` - “and”, requiring both statements to be true to return true
- `||` - “or”, requiring any of the statements to be true to return true
- `!` - the logical “not” can also be placed before a statement to invert the return value

## For Loops

For loops repeat an operation for a set number of iterations. The loop logic creates a variable, increases its value incrementally per every execution of code, and then executes the code until the var reaches a set value.

A simple `for` loop with explanation:

```js
for ( var i = 0; i < 10; i++) {
	console.log(i * 10);
}
```

- `for` keyword opens the loop
- `var i = 0;` sets the initial value of the variable
- `i < 10;` checks if the var is still less than the value at which should stop running, effectively setting the limit
- `i++` increments the var’s value on every execution
- `console.log(i * 10);` is the code that the loop will execute

This loop would print in console, iteratively `0 10 20 30 40 50 60 70 80 90` and then stop.

## While Loops

While loops repeat an operation until a set condition is met. The loop logic simply sets the condition, and then states the code to run. While loops are more flexible in their parameters, and can repeat indefinitely if necessary.

Here is the same logic as before in a `while` loop

```js
var i = 0;
while(var i < 10) {
	console.log(i * 10);
	i++
}
```

This shows that although while loops are more flexible in their accepted parameter inputs, they seem less efficient at looping when the number of iterations is known.