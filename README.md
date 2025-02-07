# Java - Script Lecture-2
### Condition - Loops - Function

### 1) Condition — это выражение, которое возвращает true (истина) или false (ложь). Условия используются для принятия решений в коде.
## Примеры условий в JavaScript:


# Condition if - else

The if-else statement is used to execute both the true part and the false part of a
given condition. If the condition is true, the if block code is executed and if the
condition is false, the else block code is executed.

```
let isRaining = true;

if (isRaining) {
    console.log("Возьмите зонт.");
} else {
    console.log("Зонт не нужен.");
}

```

# Condition Ternary Operator

An alternative to the if/else statement, the ternary operator allows JavaScript
developers to write concise conditional statements. It is written as “?:” and takes
three operands; a logical condition, a value to return if true, and a value to return if
false.
```
let age = 20;
let message = age >= 18 ? "Совершеннолетний" : "Несовершеннолетний";
console.log(message);
```
# Condition Switch case

The switch statement evaluates an expression, matching the expression's value
against a series of case clauses, and executes statements after the first case clause
with a matching value, until a break statement is encountered. The default clause of
a switch statement will be jumped to if no case matches the expression's value

```
let color = "red";

switch (color) {
    case "red":
        console.log("Красный");
        break;
    case "blue":
        console.log("Синий");
        break;
    default:
        console.log("Неизвестный цвет");
}

```
# Цикл — это конструкция, которая позволяет выполнять код много раз, пока выполняется определённое условие.

## A loop for is used when you know how many times you want to repeat an action. It consists of three parts:
```
 let cnt = "";
     for (let i = 0; i <= 10; i++) {
         cnt += num + "*" + i + "=" + num * i + "\n";
     }
     return cnt;
```
## Loop while

The while statement creates a loop that executes a specified statement as long as
the test condition evaluates to true. The condition is evaluated before executing the
statement. The following while loop iterates as long as n is less than three. 
```
let i = 1;

while (i <= 5) {
    if (i === 3) break; // Stop when i is 3
    console.log(i);
    i++;
}
```
## Loop do-while

The do...while statement creates a loop that executes a specified
statement until the test condition evaluates to false. 
```
let x = 10;

do {
    console.log("This will run ONCE");
    x++;
} while (x < 5);
```

# A function is a block of reusable code that performs a specific task. Functions are used in programming to break down complex problems into smaller, manageable parts, improving code readability and reusability.
## 1) Function Declaretion - A function is a block of reusable code that performs a specific task. Functions are used in programming to break down complex problems into smaller, manageable parts, improving code readability and reusability.
```
function sumOfDIgit(num){
    let cnt = 0;
    for(let i=0;i<=num;i++){
        cnt += i;
    }
    return cnt;
}
console.log(sumOfDIgit(12));// 24
```
## 2) Function Expretion
A function expression is a way to define a function and assign it to a variable. Unlike a function declaration, a function expression does not have a name (unless it's a named function expression) and is often used when functions need to be passed as arguments or assigned dynamically.
``` Arrow && Anonym```
### 1) Anonym 
```
const greet = function(name) {
    return `Hello, ${name}!`;
};

console.log(greet("Alice")); // Output: Hello, Alice!

```
### 2)Arrow
```
const greet = (name) => `Hello, ${name}!`;

console.log(greet("Alice")); // Output: Hello, Alice!

```
## Immediately Invoked Function Expression - is a function that runs the
moment it is invoked or called in the
JavaScript event loop. 

Having a function that behaves that way
can be useful in certain situations. IIFEs
prevent pollution of the global JS scope
```
(function greet() {
    console.log("Hello from a named IIFE!");
})();
// Output: Hello from a named IIFE!
```

# Thank you Be happy and smile 😁
