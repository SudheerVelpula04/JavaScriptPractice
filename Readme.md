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

   **Methods of Arrays**
  
    
 **1. push(item1, item2, ...):** Adds one or more elements to the end of the array.
  
    
                    let myArray = [1, 2, 3];
                  myArray.push(4, 5);
                  // myArray is now [1, 2, 3, 4, 5]
  
  **2. pop():** Removes and returns the last element of the array.
  
                  let myArray = [1, 2, 3, 4, 5];
                  let poppedElement = myArray.pop(); // Returns 5
                  // myArray is now [1, 2, 3, 4]
                  
  **3. shift():** Removes and returns the first element of the array.
  
                  let myArray = [1, 2, 3, 4, 5];
                  let shiftedElement = myArray.shift(); // Returns 1
                  // myArray is now [2, 3, 4, 5]
  
  **4. unshift(item1, item2, ...)**: Adds one or more elements to the beginning of the array.
  
                let myArray = [2, 3, 4, 5];
                myArray.unshift(0, 1);
                // myArray is now [0, 1, 2, 3, 4, 5]

                
  **5. concat(array1, array2, ...):** Combines two or more arrays, returning a new array.
  
                let array1 = [1, 2, 3];
                let array2 = [4, 5, 6];
                let combinedArray = array1.concat(array2);
                // combinedArray is [1, 2, 3, 4, 5, 6]
  
  **6. slice(startIndex, endIndex)**: Returns a shallow copy of a portion of the array.
  
              let myArray = [1, 2, 3, 4, 5];
              let slicedArray = myArray.slice(1, 4); // Returns [2, 3, 4]
  
  **7. splice(startIndex, deleteCount, item1, item2, ...):** Changes the contents of an array by removing or replacing existing elements and/or adding new elements.

  
              let myArray = [1, 2, 3, 4, 5];
              myArray.splice(2, 2, 6, 7); // Removes elements at index 2 and 3, adds 6 and 7
              // myArray is now [1, 2, 6, 7, 5]
              
  **8. forEach(callback(item, index, array)):** Executes a provided function once for each array element.

  
              let myArray = [1, 2, 3];
              myArray.forEach(function(item, index) {
                  console.log(item, index);
              });

              
   **9. filter(callback(item, index, array)):** Creates a new array with all elements that pass the test implemented by the provided function.

   
               let myArray = [1, 2, 3, 4, 5];
              let filteredArray = myArray.filter(function(item) {
                  return item > 2;
              });
              // filteredArray is [3, 4, 5]
              
              
  **10. map(callback(item, index, array))**: Creates a new array with the results of calling a provided function on every element.

  
                  let myArray = [1, 2, 3];
              let squaredArray = myArray.map(function(item) {
                  return item * item;
              });
              // squaredArray is [1, 4, 9]
              
  
  **11. reduce(callback(accumulator, item, index, array), initialValue):** Applies a function against an accumulator and each element, reducing the array to a single value.

  
              let myArray = [1, 2, 3, 4, 5];
              let sum = myArray.reduce(function(accumulator, item) {
                  return accumulator + item;
              }, 0);
              // sum is 15
              
  **12. indexOf(item, startIndex):** Returns the first index at which a given element can be found in the array, or -1 if it is not present.
  
              let myArray = [10, 20, 30, 40, 50];
              let index = myArray.indexOf(30); // Returns 2
              
  **13. includes(item, startIndex):** Determines whether the array contains a certain element, returning a boolean value.

  
              let myArray = [10, 20, 30, 40, 50];
              let includesElement = myArray.includes(30); // Returns true
  
              
  **14. every(callback(item, index, array)):** Checks if every element in the array passes a given test.

  
              let myArray = [10, 20, 30, 40, 50];
              let allGreaterThanFive = myArray.every(function(item) {
                  return item > 5;
              }); // Returns true
  
              
  **15. some(callback(item, index, array)):** Checks if at least one element in the array passes a given test.

  
              let myArray = [10, 20, 30, 40, 50];
              let anyGreaterThanThirty = myArray.some(function(item) {
                  return item > 30;
              }); // Returns true
  
              
  **16. sort(compareFunction):** Sorts the elements of an array in place and returns the sorted array.

  
                let myArray = [3, 1, 4, 1, 5, 9, 2, 6];
                myArray.sort(); // Sorts numerically: [1, 1, 2, 3, 4, 5, 6, 9]
  
                
  **17. reverse():** Reverses the order of elements in an array.

  
              let myArray = [1, 2, 3, 4, 5];
              myArray.reverse(); // Reverses the array: [5, 4, 3, 2, 1]
  
              

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

# Sorting Arrays:
**1 .sort():**

The sort() method in JavaScript is used to sort the elements of an array in place and returns the sorted array. By default, it converts elements to strings and sorts them based on their UTF-16 code unit values. However, you can provide a custom sorting function to define your own sorting criteria.

              let fruits = ["banana", "apple", "orange", "grape"];
              fruits.sort();
              console.log(fruits); // Output: ["apple", "banana", "grape", "orange"]

By default, the **sort()** method sorts elements as strings. This can lead to unexpected results when sorting numbers:

          let numbers = [10, 2, 30, 5];
          numbers.sort();
          console.log(numbers); // Output: [10, 2, 30, 5] (not in numerical order)
          
To sort numbers numerically, you can provide a custom sorting function: 

              let numbers = [10, 2, 30, 5];
              numbers.sort(function(a, b) {
                  return a - b;
              });
              console.log(numbers); // Output: [2, 5, 10, 30]
**2.Numeric Sort:**

By default, the **sort()** function sorts values as **strings**.

This works well for strings ("Apple" comes before "Banana").

However, if numbers are sorted as strings, "25" is bigger than "100", because "2" is bigger than "1".

Because of this, the sort() method will produce incorrect result when sorting numbers.

You can fix this by providing a **compare function**:

**1.Ascending Numeric Sort:**

                        let numbers = [10, 2, 5, 8, 1];
                        numbers.sort(function(a, b) {
                            return a - b;
                        });
                        
                        console.log(numbers); // Output: [1, 2, 5, 8, 10]

In the comparison function function(a, b) { return a - b; }, if the result is negative, a will be placed before b. If it's positive, b will be placed before a. If the result is zero, the order remains unchanged.

**2. Descending Numeric Sort:**

                      let numbers = [10, 2, 5, 8, 1];
                      numbers.sort(function(a, b) {
                          return b - a;
                      });
                      
                      console.log(numbers); // Output: [10, 8, 5, 2, 1]
                      
**3. Simplified Arrow Function (ES6+):**

                      let numbers = [10, 2, 5, 8, 1];
                      let sortedNumbers = numbers.slice().sort((a, b) => a - b);
                      
                      console.log(sortedNumbers); // Output: [1, 2, 5, 8, 10]
                      console.log(numbers); // Original array remains unchanged: [10, 2, 5, 8, 1]
# JavaScript Array Iteration methods 

**1. forEach()**: Executes a provided function once for each array element.

                    let numbers = [1, 2, 3, 4, 5];
                    numbers.forEach(function(number) {
                        console.log(number);
                    });

**2. map():** Creates a new array with the results of calling a provided function on every element.

                let numbers = [1, 2, 3];
                let squaredArray = numbers.map(function(number) {
                    return number * number;
                }); // [1, 4, 9]
                
**3. filter():** Creates a new array with all elements that pass the test implemented by the provided function.

                        let numbers = [1, 2, 3, 4, 5];
                  let evenNumbers = numbers.filter(function(number) {
                return number % 2 === 0;
                  }); // [2, 4]

  **4. reduce():** Applies a function against an accumulator and each element in the array, reducing it to a single value.      

                let numbers = [1, 2, 3, 4, 5];
                let sum = numbers.reduce(function(accumulator, number) {
                    return accumulator + number;
                }, 0); // 15

**5. some():** Checks if at least one element in the array passes a test implemented by the provided function.

                let numbers = [1, 2, 3, 4, 5];
                let hasEven = numbers.some(function(number) {
                    return number % 2 === 0;
                }); // true

                
**6. every():** Checks if all elements in the array pass a test implemented by the provided function.


                  let numbers = [2, 4, 6, 8, 10];
                  let allEven = numbers.every(function(number) {
                      return number % 2 === 0;
                  }); // true

**7. find():** Returns the first element in the array that satisfies the provided testing function.

                let numbers = [1, 2, 3, 4, 5];
                let firstEven = numbers.find(function(number) {
                    return number % 2 === 0;
                }); // 2

                
**8. findIndex():** Returns the index of the first element in the array that satisfies the provided testing function.

                let numbers = [1, 2, 3, 4, 5];
                let firstEvenIndex = numbers.findIndex(function(number) {
                    return number % 2 === 0;
                }); // 1 (index of number 2)


