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
The first sum will return the value but the second sum will be logged into the console and it will show undefined.

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
It will throw undefined.

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
The output will be order of the first two parameters only.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
Yes, we can store it as we are returning a value so it can be stored in a variable.

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
```js
function sayHello(name){
  return `Hello ${name}`;
}
sayHello("Arya");
```

6. What will be the output of the function below and why?
The output will be `Hello John`, as the variable `userName` is already defined.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // It will alert the userName `John`;

showMessage(); // It will return the message `Hello John`;

alert(userName); // It will throw a reference error as variable userName is not defined inside the function's body.
```

8. What is a Anonymous Function give example of three functions.
The functions that are not names are known as anonymous functions. For example;
```js
let example = function(a,b){
  return a + b;
}
```

9. Can function declaration be a Anonymous Function? Explain
Yes, function declaration could be an Anonymous Function as it is not important to name each and every function declaration.

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.
```js
function getData(name){
  return `${name} is me!`;
}
```
```js
function addNum(a, b){
  return a + b;
}
```
```js
fucntion subNum(a, b){
  return a - b;
}
```
```js
function mulNum(a, b){
  return a * b;
}
```
```js
function checkValue(a){
  if(a >= 0){
    return true;
  }else {
    return false;
  }
}
```
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
