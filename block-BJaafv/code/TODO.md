1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```
The first sum function will be returning a value i.e. the sum and the second one will be putting the output on the console and does not return anything.

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
The first function has a return type so will store the sum of the arguments sent and the second one does not have a return type so will be an error . And both will show undefined on console tillwe have notcalled them.

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
The output will be 36; as there are only two parameters so the first two values will be considered.


4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
Yes we can store it in variable because it has a return statemen hence value will be returned.

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
```js
function sayHello(name){
  let message="hello"+name;
return message;
}
```

6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```
The output will be `Hello, John` because the function has a return statement ehich returns the message.

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // Output 1
//`John` will be output because username is declared outside the function and it is accessible.

showMessage(); // Output 2 This will return the value `Hello,John` as there is a return statement.

alert(userName); // Output 3`John` will be the output as the username value will only be alerted.
```

8. What is a Anonymous Function give example of three functions.
Anonymous function expression is a function whose value is stored in a variable or constant. It is anonymous because we don not need to provide a function name here as the function value can be referred with the variable name.eg.

const address=function(a,b){
  return a+b;
};
const add=function(a,b){
  return a+b;
};
const address=(a,b)=>return a+b;

9. Can function declaration be a Anonymous Function? Explain
Yes a function declaration be anonymous function. This function can be called using the variable name in which the function value is stored hence the name for function is not needed.

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```
5 example of good naming convention for defining a function are:
1. Function name should be verb , usually describing the task it is doing.
2. It should start with a vebal prefix.
3. it should not start with a number.
4. It is better if we use camelCase while naming them.
5. We can also use _ .