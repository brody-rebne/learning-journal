[Home](https://zx37.github.io/learning-journal/)

# JavaScript Objects and Expressions

## Scripts

Scripts are coded instructions for a computer built to achieve a specific goal. They are what manipulates raw content to make pages and apps dynamic. Scripts must be specific in language and syntax so that no assumptions are made. Entities must be carefully defined and described, and instructions must be clear and complete.

A simple script in human syntax could be something as setting a variable (`var x = 12`), or a more complicated logical function, like this one below that finds and displays the time in a page:

```js
function updateTime() {
    var today = new Date();
    var hour = today.getHours();
    var min = today.getMinutes();
    var sec = today.getSeconds();
    
    if (min < 10) {
        min = '0' + min;
    }
    if (sec < 10) {
        sec = '0' + sec;
    }
    
    var time = hour + ':' + min + ':' + sec;

    document.write(time);
}
```

## Expressions

Expressions are the operational syntax of JavaScript. They instruct the computer what to do with the information given to them. Some common operators are:

- `=` - sets the value of a variable
- `+, -, *, /` - basic mathmatical operators
- `++, --` - increments a number by 1
- `==` - checks if two items hold the same value
- `===` - checks if two items hold the same strictly-typed value
- `!=, !==` - "not" versions of `==` and `===`
- `<, >, <=, >=` - checks if one value is greater/less (+or equal to) another
- `||` - applies "or" conditionality
- `&&` - applies "and" conditionality

## Functions

Functions are reusable wrappers for code blocks of logic that return a value upon completion. A function is declared like so:

```js
function newFunction() {
    code.doSomething;
}
```
And can be called, or run on command, in many different ways. The simplest, basic way to call them is by saying:

```js
newFunction();
```

## Putting the Pieces Together

Knowing all this, we can break down and interpret the function above.

```js
//initializing the function
function updateTime() {
    //declaring variables and giving them values.
    //the first var is given a value determined by a built in function
    //the rest are determined by methods, an object like a function but where the logic is performed on a variable or other entity.
    //you can see that we've gotten todays date/time on the first line, and then made vars containing the hour, minute, and second components of that date/time.
    var today = new Date();
    var hour = today.getHours();
    var min = today.getMinutes();
    var sec = today.getSeconds();
    
    //here we add an additional 0 to the minutes and seconds if they are less than 10, so that 9:03:08 doesn't render as 9:3:8.
    if (min < 10) {
        min = '0' + min;
    }
    if (sec < 10) {
        sec = '0' + sec;
    }
    //here we create a final var semantically combining values and separators into a single string.
    var time = hour + ':' + min + ':' + sec;
    //finally, we write that last variable directly into the html, wherever the script is pointed at in the html.
    document.write(time);
}