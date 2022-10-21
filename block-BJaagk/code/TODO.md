1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here

let fun1 = function(marks, total) {
  return (marks * 100) /total;
}

let fun2 = (marks, total) => {
  return (marks * 100) / total;
}

```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer

let fun3 = function(marks, total) {
  return (marks*100)/total;
}
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};


function fun4(marks, total) {
  return (marks *100) / total;
}
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};


function fun5(marks, total) {
  return (marks*100) / total;
}
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};


function fun6(marks, total) {
  return (marks*100)/total;
}
```

```js
let percentage = (marks, total) => (marks * 100) / total;
function fun7(marks, total) {
  return (marks*100)/total;
}
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
- cause it is an object

4. Why is a function call an expression in JavaScript?
- returns a value


5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // VALID
five = add; // VALID
five = five(10, 11); // VALID
five = function () {
  return 'Hello';
}; // VALID
```

6. What is the difference between function definition and function call? Explain with an example.

7. What is the similarities between function definition and function call?

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // VALID
```

9. What is higher order function explain with an example.
- Takes one or more function as argument.


10. Explain what is callback function. Why you can pass a function inside a function?
