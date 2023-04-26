1. Using loops take 10 inputs from user and find the average of all the numbers.
```js
for(let i = 0; i > 10; i++){
  let num = parseInt(prompt("Enter a number: "));
  console.log(num);
  }
  let sum = 0;
  for(let i = 0; i < 10; i++){  
    sum += parseInt(prompt("Enter a number: "));
    } 
    console.log("The average is: " + sum / 10);
    ```

2. What will be the output of the code below.
js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```
printIn is not defined

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
```js
function getEvenSum(max == 10){
  let sum = 0;
  for (let i = 0; i < max; i++) {
    if (i % 2 === 0) {
      sum += i;
      }
      }
      return sum;
      }
      getEvenSum();
      ```
4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
```js
function getOddSum(max == 10){
  let sum = 0;
  for (let i = 0; i < max; i++) {
    if (i % 2 !== 0) {
      sum += i;
      }
      }
      return sum;
      }
      getOddSum();
      ```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.
```js 
function getProductOfDigits(num){
  let product=1;
  for(let i=1;i<=num.length;i++){
    product=product*i;
  }
  if(product<0){
    return `not a valid input`
  }else{
    return product
  }

}
getProductOfDigits("123")
```
- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); // Bigger than 5
check(1); // Smaller than 5
check(5); // 5
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // 'You are arya'because  we are returning the value 
getOutput('John'); //'You are John 'because  we are returning the value 
getOutput(); // 'Who are you'
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // it will consolelog arya and also return the value
getOutput('John'); // it will consolelog john and also return the value
getOutput(); // "Who are you" because  we are returning the value 
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
yes function can have multiple return statements,
```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}
```
10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
The JavaScript 'for loop' iterates the elements for the fixed number of times. It should be used if number of iteration is known.
```js
for(let i = 0; i > 10; i++){
  console.log(i);
}
```
The JavaScript 'while loop' iterates the elements for the infinite number of times. It should be used if number of iteration is not known.
```js
while(i > 10){
  console.log(i);
}
```