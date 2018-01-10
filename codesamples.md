1. A nested function that prints a stack trace error to the console


````

function firstFunction(){
throw new Error('Stack Trace Error');
}

function secondFunction(){
firstFunction();
}

function thirdFunction(){
secondFunction();
}

thirdFunction();


````


2. A function that calls another function to show how the stack handles multiple function calls.

````

function firstFunction(){
 console.log("Hello from firstFunction");
}

function secondFunction(){
 firstFunction();
 console.log("The end from secondFunction");
}

secondFunction();

````

3. A recursive function that will throw a maxiumu call stack error.

````
function callMyself(){
  callMyself();
}

callMyself();

````
