# Introduction-to-JavaScript

### **Session Plan: Introduction to JavaScript**

---

### **Introduction and Setup**
1. **Introduction to JavaScript**
   - **What is JavaScript?**
     - JavaScript is a high-level, dynamic programming language commonly used in web development.
     - Runs in the browser to make web pages interactive.
   - **Real-world examples**: Interactive forms, dynamic content updates, animations.
   
2. **Setting Up the Environment**
   - **Browser Console**: Open the console in a web browser (e.g., Chrome: Right-click -> Inspect -> Console).
   - **Text Editor**: Recommend VS Code or Sublime Text.
   - **Basic HTML File**:
     ```html
     <!DOCTYPE html>
     <html>
     <head>
       <title>JavaScript Basics</title>
     </head>
     <body>
       <script src="script.js"></script>
     </body>
     </html>
     ```

---

### **JavaScript Basics**
1. **Hello, World!**
   - **Example**: 
     ```javascript
     alert('Hello, World!');
     ```
   - Run in the browser console or in an HTML file.

2. **Variables**
   - **Declaration**:
     ```javascript
     let name = 'John';
     const pi = 3.14;
     var age = 30;
     ```
   - **Example**:
     ```javascript
     let message = 'Hello, ' + name;
     alert(message);
     ```

3. **Data Types**
   - **Numbers**:
     ```javascript
     let x = 5;
     let y = 10.5;
     ```
   - **Strings**:
     ```javascript
     let greeting = 'Hello';
     ```
   - **Booleans**:
     ```javascript
     let isActive = true;
     ```
   - **Example**:
     ```javascript
     let age = 25;
     let isAdult = age >= 18;
     alert(isAdult); // true
     ```

---

### **Basic Operations and Interaction**
1. **Operators**
   - **Arithmetic**:
     ```javascript
     let sum = 5 + 3; // 8
     let difference = 5 - 3; // 2
     let product = 5 * 3; // 15
     let quotient = 5 / 3; // 1.666...
     ```
   - **Assignment**:
     ```javascript
     let x = 10;
     x += 5; // x is now 15
     ```

2. **User Interaction**
   - **alert**:
     ```javascript
     alert('This is an alert!');
     ```
   - **prompt**:
     ```javascript
     let name = prompt('What is your name?');
     alert('Hello, ' + name);
     ```
   - **confirm**:
     ```javascript
     let isSure = confirm('Are you sure?');
     alert(isSure); // true or false
     ```

---

### **Conditionals and Loops**
1. **Conditionals**
   - **if, else, else if**:
     ```javascript
     let age = prompt('How old are you?');
     if (age >= 18) {
       alert('You are an adult.');
     } else if (age > 12) {
       alert('You are a teenager.');
     } else {
       alert('You are a child.');
     }
     ```

2. **Loops**
   - **for**:
     ```javascript
     for (let i = 0; i < 5; i++) {
       console.log(i);
     }
     ```
   - **while**:
     ```javascript
     let i = 0;
     while (i < 5) {
       console.log(i);
       i++;
     }
     ```
   - **do...while**:
     ```javascript
     let i = 0;
     do {
       console.log(i);
       i++;
     } while (i < 5);
     ```

---

### **Functions**
1. **Function Declaration**
   - **Example**:
     ```javascript
     function greet(name) {
       alert('Hello, ' + name);
     }
     greet('Alice');
     ```

2. **Function Expressions and Arrow Functions**
   - **Function Expression**:
     ```javascript
     const add = function(a, b) {
       return a + b;
     };
     console.log(add(2, 3)); // 5
     ```
   - **Arrow Function**:
     ```javascript
     const multiply = (a, b) => a * b;
     console.log(multiply(2, 3)); // 6
     ```

---

### **Objects and Arrays**
1. **Objects**
   - **Creation and Access**:
     ```javascript
     let person = {
       name: 'John',
       age: 30,
       greet: function() {
         alert('Hello, ' + this.name);
       }
     };
     alert(person.name); // John
     person.greet(); // Hello, John
     ```

2. **Arrays**
   - **Creation and Manipulation**:
     ```javascript
     let colors = ['red', 'green', 'blue'];
     colors.push('yellow');
     console.log(colors); // ['red', 'green', 'blue', 'yellow']
     console.log(colors[0]); // red
     ```

---

### **Loops in Arrays**

1. **Using `for` Loop**:
   - **Example**:
     ```javascript
     let colors = ['red', 'green', 'blue', 'yellow'];
     for (let i = 0; i < colors.length; i++) {
       console.log(colors[i]);
     }
     ```

2. **Using `for...of` Loop**:
   - **Example**:
     ```javascript
     let colors = ['red', 'green', 'blue', 'yellow'];
     for (let color of colors) {
       console.log(color);
     }
     ```

3. **Using `forEach` Method**:
   - **Example**:
     ```javascript
     let colors = ['red', 'green', 'blue', 'yellow'];
     colors.forEach(function(color) {
       console.log(color);
     });
     ```
     
