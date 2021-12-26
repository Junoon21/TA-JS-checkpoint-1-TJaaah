1. Using loops take 10 inputs from user and find the average of all the numbers.
for(let i=0;i<10;i++){
var sum=Number(prompt("enter value"));
sum+=sum;
}
let average=sum/i;
2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```
hihihi
3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
function getEvenSum(max=10){
  for(let i=0;i<max;i++>){
    if(i%2===0){
      var sum=sum+i;
    }
  }
}
4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
function getOddSum(max=10){
  for(let i=0;i<max;i++>){
    if(i%2===0){
      var sum=sum+i;
    }
  }
}
5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.
function getProductOfDigits(num){
  if(num<0)
  {
    return("not a valid input");
  }
  else {
    while(num!=0){
      var product=1;
      var last_digit=num%10;
      product=product*last_digit;
      num=num/10;
    }
  }

}
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

check(10); // 'Bigger than 5' will be the output because the return statement ends function execution and returns value.
check(1); // Smaller than 5' will be the output because the return statement ends function execution and returns value.
check(5); // 5 because upper two conditions will be false.
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // 'You are arya' is the output as after return statement ends function execution and returns value.
getOutput('John'); // 'You are john is the output as after return statement ends function execution and returns value.
getOutput(); //'Who are you" will be returned as no value is being sent so the last return statement will be used.
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // 'You are arya'will be output in console and  'Who are you' will be returned.
getOutput('John'); // 'You are john'will be output in console and  'Who are you' will be returned.
getOutput(); // 'Who are you'will be returned as this is the return value and no other condition is true.
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
Yesa function van have multiple return statement based on which condition will return what. Different conditions will have different outputs, hence multiple return statements are possible .eg.
function applianceToBuy(appliance){
  switch(appliance){
    case `tv`:return("you bought a tv");
    break;
     case `phone`:return("you bought a phone");
    break;
     case `refrigerator`:return("you bought a refrigerator");
    break;
     case `fridge`:return("you bought a fridge");
    break;
    default:return("your appliance is not available");
  }
}
10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
For loop is used when the number of iteration is known.Here initialisation takes place only once . In absense of condition the loop iterates infinite times and stops when break command is reached.Used when number of iterations is known.
While loop is used when the number of iterations is unknown . The loop goes on till the condition becomes false and here initialisation is done everytime the loop is iterated. In absense of condition the loop shows error.