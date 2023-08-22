# JavaScriptPractice
Java
# What is JavaScript?
java Script is a dynamically typed programming lang primarily used for adding interactivity dynamic content and behavior to websites and applications and we called a single third lang.
# Who invented JavaScript?
JavaScript was invented by Brendan Eich in 1995. It was developed for Netscape 2, and became the ECMA-262 standard in 1997. 
# features-of-javascript
**Scripting**:
Javascript executes the client-side script in the browser.

**Interpreter**:
The browser interprets JavaScript code.

**Event Handling:**
Events are actions. Javascript provides event-handling options.

**Light Weight:**
  As Javascript is not a compiled language, source code never changes to byte code before running time. Low-end devices can also run Javascript because of its lightweight feature.
  
**Case Sensitive:**
  In Javascript, names, variables, keywords, and functions are case-sensitive.
  
**Control Statements:**
   Javascript has control statements like if-else-if, switch case, and loop. Users can write complex code using these control statements.

**Objects as first-class Citizens:**
   Javascript arrays, functions, and symbols are objects which can inherit the Object prototype properties. Objects being first-class citizens means Objects can do all tasks.

**Supports Functional Programming:**
    Javascript functions can be an argument to another function, can call by reference, and can assign to a variable.

**Dynamic Typing:**
    Javascript variables can have any value type. The same variable can have a string value, an integer value, or any other.

**Client-side Validations:**
    Javascript client-side validations allow users to submit valid data to the server during a form submission.

**Platform Independent:**
    Javascript will run in the same way in all systems with any operating system.

**Async Processing:**
    Javascript async-await and promise features provide asynchronous nature. As the processes run in parallel, it improves processing time and responsiveness.

**Prototype-based:**
    Javascript follows 'Object.prototype' functions instead of class inheritance.

**Nullish Coalescing Operator (??):**
    The nullish coalescing operator returns the right side operand if the left side operand is null. If the left operand is not 'null', the operator returns the left side operand value. This operator helps to 
     avoid Boolean operator errors.

**Logical nullish assignment (??=):**
It is the shorthand of

          result=left??right;

**Styling Console Log:**
Javascript consoles can have styles. For example, see the block below.

          console.log('%cText %cValue', 'color:black; cursor:pointer', 'color: green;');

The first set of styles applies to the first string with %c, and the second %c gets the second style set for the second string.

**Object Shorthand:**
Object shorthand can save space and time by allowing users to use the same name for assigning variables and key values.
# Data Types :
**Primitive:** its mean immutable dataType.


**1. Number:** Represents both integer and floating point numbers.

        '5','4.15'
        
  **2. String:**   Represents a Sequence of characters
  
         'hello' , "Hello"

  **3. Boolean:**  Represents a 'true' are 'false'

           'true' are 'false'          
           
 **4.undefined:**  Represents a variable that has been declared but not assigned a value

          undefind

**5 .null:** Represents a intentional absence of any value

          null

**Non-Primitive(or)Complex DataTypes:** its mean mutable dataType.

**1. Objects:** Represents a collection of key-value pairs, where keys are strings (or symbols) and values can be of any data type. Objects can be used to represent various structures like arrays, functions, and custom-defined types.

        { name: 'John', age: 30 }
        
**2. Arrays:** Represents an ordered list of values, accessed using numerical indices.

             [1,2,3,4]

**3. Functions:** Represents a block of reusable code that can be invoked with arguments to perform a specific task. Functions are also objects in JavaScript.

            function add(a, b) {
              return a + b;
              }
  # operators in JavaScript:

 **1. Arithmetic Operators:**
These operators perform basic arithmetic operations on numerical values.

  Addition(+),
  Subtraction(-),
  Multiplication(*),
  Division(/),
  Modulus (remainder)(%),
  Exponentiation (ES6)(**).

            let a = 10;
            let b = 3;
            
            console.log(a + b); // 13
            console.log(a - b); // 7
            console.log(a * b); // 30
            console.log(a / b); // 3.333...
            console.log(a % b); // 1
            console.log(a ** b); // 1000 (a raised to the power of b)

**2.Assignment Operators:**
These operators assign values to variables.

 Assigns a value(=),
 Adds and assigns(+=),
 Subtracts and assigns(-=),
 Multiplies and assigns(*=),
 Divides and assigns(/=)
 Modulus and assigns(%=)
 Exponentiation and assigns (ES6)(**=)

              let x = 5;
              x += 3; // equivalent to x = x + 3
              console.log(x); // 8
              
              let y = 10;
              y *= 2; // equivalent to y = y * 2
              console.log(y); // 20

**3.Comparison Operators:**
These operators compare two values and return a Boolean result (true or false).

 Equal to(==),
 Not equal to(!=),
 Strictly equal to(===),
 Strictly not equal to(!==),
 Greater than(>),
 Less than(<),
 Greater than or equal to(>=),
 Less than or equal to(<=).


                let p = 5;
                let q = "5";
                
                console.log(p == q); // true (loose equality, coerces types)
                console.log(p === q); // false (strict equality, compares types)
                console.log(p != q); // false
                console.log(p !== q); // true
                console.log(p > 3); // true
                console.log(p < 3); // false

**4.Logical Operators:**
These operators are used to combine or manipulate Boolean values.

Logical AND(&&),
Logical OR(||),
Logical NOT(!).

                let isTrue = true;
                let isFalse = false;
                
                console.log(isTrue && isFalse); // false (logical AND)
                console.log(isTrue || isFalse); // true (logical OR)
                console.log(!isTrue); // false (logical NOT)

**5.Conditional (Ternary) Operator:**
This operator is a shorthand for an if-else statement.

                let age = 17;
                let status = (age >= 18) ? "Adult" : "Minor";
                console.log(status); // "Minor"


**6.Type Operators:**

**typeof** Returns a string indicating the type of a value

**instanceof** Checks if an object is an instance of a particular class

                console.log(typeof 42);        // "number"
                console.log(typeof "hello");   // "string"
                console.log(typeof true);      // "boolean"
                
                let arr = [1, 2, 3];
                console.log(arr instanceof Array); // true

# Conditional Statements:

onditional statements in JavaScript allow you to execute different blocks of code based on whether a certain condition is true or false. These statements are crucial for creating dynamic and responsive programs. There are mainly three types of conditional statements in JavaScript: if statements, else if statements, and switch statements.

**1. if Statement:**

The if statement is the most basic form of a conditional statement. It evaluates a given condition and, if the condition is true, executes the code inside the block that follows.


            if (condition) {
                // Code to be executed if the condition is true
            }


              let age = 18;
              if (age >= 18) {
                  console.log("You are eligible to vote.");
              }

           
**2. if...else Statement:**

The if...else statement allows you to provide an alternative block of code to execute when the condition is false.

            if (condition) {
                // Code to be executed if the condition is true
            } else {
                // Code to be executed if the condition is false
            }

            Examp:
            let temperature = 25;
            if (temperature > 30) {
                console.log("It's hot outside.");
            } else {
                console.log("It's not too hot.");
            }
**3.else if Statement:**

The else if statement lets you check multiple conditions in sequence and execute the corresponding block of code for the first true condition.

              if (condition1) {
                  // Code to be executed if condition1 is true
              } else if (condition2) {
                  // Code to be executed if condition2 is true
              } else {
                  // Code to be executed if no conditions are true
              }


              let score = 85;
              if (score >= 90) {
                  console.log("You got an A.");
              } else if (score >= 80) {
                  console.log("You got a B.");
              } else {
                  console.log("You got a lower grade.");
              }

**4. switch Statement:**

The switch statement is used when you have a specific value to compare against multiple possible cases. It's a cleaner alternative to using multiple if...else statements.

            switch (expression) {
                case value1:
                    // Code to be executed if expression matches value1
                    break;
                case value2:
                    // Code to be executed if expression matches value2
                    break;
                // ...
                default:
                    // Code to be executed if no cases match expression
            }

            Examp:
            let day = "Monday";
            switch (day) {
                case "Monday":
                    console.log("It's the start of the week.");
                    break;
                case "Friday":
                    console.log("Its a WeekEnd");
                    break;
                default:
                    console.log("It's a regular day.");
            }




# function:
A JavaScript **function** is a block of code designed to perform a particular task. A JavaScript function is executed when "something" invokes it (calls it).

**Function Keyword:**
The keyword function is used to define a function in JavaScript.

**Function Name:**
This is the name you give to your function. It's used to call the function later when you want to execute the code within it.

**Parameters:**
These are optional variables listed in the parentheses after the function name. They act as placeholders for values that you can pass to the function when calling it. You can have zero or more parameters.

**Function Body:**
This is the block of code enclosed in curly braces {}. It contains the instructions that will be executed when the function is called. You can use the parameters and define local variables within the function body.

**Return Statement:**
If you want your function to produce an output, you can use the **return** statement to specify the value that the function should return. If the **return** statement is omitted, the function will return **undefined**.


            function add(a, b) {
              return a + b;
            }
            
            let result = add(3, 5); // Calling the function and storing the result
            console.log(result);    // Output: 8


In this example, the function **add** takes two parameters, **a** and **b**, and returns their sum. When you call **add(3, 5)**, it returns **8**, which is then stored in the variable **result**.



#  Type Casting:

Type casting in JavaScript, also known as type conversion, refers to the process of changing the data type of a value from one type to another. JavaScript performs automatic type coercion in many cases, but explicit type casting allows you to control how values are converted from one type to another.

There are two main types of type casting in JavaScript:

**1.Implicit Type Casting (Type Coercion):**

JavaScript automatically converts values from one type to another in certain situations. This often happens in operations involving different data types.

              let num = 5 + "10"; // JavaScript coerces the number to a string
              console.log(num);   // Output: "510"
In this example, the number 5 is implicitly converted to a string and then concatenated with the string "10".

**2. Explicit Type Casting:**

Explicit type casting involves converting a value from one type to another using built-in functions or operators. There are several methods for explicit type casting in JavaScript:

**parseInt()** and **parseFloat()**: Convert strings to integers or floating-point numbers.

**Number()**: Converts a value to a number, regardless of its original type.

**String()**: Converts a value to a string.

**Boolean()**: Converts a value to a boolean.

**toString()**: Converts a value to its string representation.

Example using **Number()**:

            let str = "42";
            let num = Number(str); // Explicitly converting string to number
            console.log(num);      // Output: 42

Example using **String():**

            let value = 123;
            let strValue = String(value); // Explicitly converting number to string
            console.log(strValue);       // Output: "123"
            
Example using **Boolean():**

            let truthyValue = "hello";
            let boolValue = Boolean(truthyValue); // Explicitly converting string to boolean
            console.log(boolValue);              // Output: true


# loops

used in JavaScript to perform repeated tasks based on a condition

**1 .for Loop:**
For loop is used to iterate a set of statements based on a condition.
            
            for(Initialization; Condition; Increment/decrement){  
            //code  
            } 
            for(var i=0; i<=9;i++){
            console.log("sudheer");
            }

**2 .While Loop:**
While is also used to iterate a set of statements based on a condition. Usually while is preferred when number of iterations are not known in advance.

              while (condition) {  
                // code 
              }  

              
              let i=1 
              while (i<=100){
              if(i%2==0){
              console.log(i)
              }
              i++
              }

**3 .Do While Loop:**
    Do-while is also used to iterate a set of statements based on a condition. It is mostly used when you need to execute the statements atleast once.



            do {  
              // code 
            } while (condition); 

            
            let EvenNum=1;
                do {
                    console.log("THis is Even Num",EvenNum);
                    EvenNum +=2;

                }while (EvenNum <=100);

# string methods:

The **String** object is used to represent and manipulate a sequence of characters.


**1.length:** Returns the length of the string.
                
                const str = "Hello, World!";
                console.log(str.length); // Outputs: 13


**2. toUpperCase()** and **toLowerCase():** Converts the string to uppercase or lowercase.


            const str = "Hello, World!";
            console.log(str.toUpperCase()); // Outputs: "HELLO, WORLD!"
            console.log(str.toLowerCase()); // Outputs: "hello, world!"

**3. charAt(index):** Returns the character at the specified index.

            const str = "Hello";
            console.log(str.charAt(0)); // Outputs: "H"
            console.log(str.charAt(2)); // Outputs: "l"


**4. substring(start, end):** Returns a substring starting from the start index and ending before the end index.

          const str = "Hello, World!";
          console.log(str.substring(7, 12)); // Outputs: "World"
          
**5. slice(start, end):** Similar to **substring**, but can also work with negative indices.

                const str = "Hello, World!";
                console.log(str.slice(7, 12)); // Outputs: "World"



**6. indexOf(substring, fromIndex)** and **lastIndexOf(substring, fromIndex):** Finds the index of the first or last occurrence of the specified substring, starting from **fromIndex**.

                
                const str = "Hello, World!";
                console.log(str.indexOf("World")); // Outputs: 7
                console.log(str.lastIndexOf("l")); // Outputs: 9
**7. startsWith(prefix)** and **endsWith(suffix):** Checks if the string starts with the specified prefix or ends with the specified suffix.

                const str = "Hello, World!";
                console.log(str.startsWith("Hello")); // Outputs: true
                console.log(str.endsWith("World!")); // Outputs: true
                
**8. replace(oldValue, newValue):** Replaces occurrences of **oldValue** with **newValue**.

              const str = "Hello, World!";
              const newStr = str.replace("World", "Universe");
              console.log(newStr); // Outputs: "Hello, Universe!"

**9. split(separator, limit):** Splits the string into an array of substrings based on the **separator**. 


                const str = "apple,banana,grape";
                const arr = str.split(",");
                console.log(arr); // Outputs: ["apple", "banana", "grape"]

**10. trim():** Removes leading and trailing whitespace characters from the string.

                  const str = "   Hello, World!   ";
                  console.log(str.trim()); // Outputs: "Hello, World!"

