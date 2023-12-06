 # SOLUTION
 
 ## Loops
Loops are control structures in programming that allow a set of instructions to be repeated multiple times. They are essential for automating repetitive tasks, iterating over collections of data, and performing operations until a certain condition is met.

**There are several types of loops in most programming languages, including:**

1. **`For Loop:`**

  - Syntax :
           ```bash
           for (initialization; condition; update) {
           // Code to be executed in each iteration
          }

           ```

   - Example :
           ```js
           for (let i = 0; i < 5; i++) {
              console.log(i);
            }

          ```


2. **`While Loop:`**

  - Syntax :
           ```bash
           while (condition) {
            // Code to be executed as long as the condition is true
          }
        ```

  - Example :
           ```js
           let i = 0;
           while (i < 5) {
               console.log(i);
               i++;
           }
           ```


3. **`Do-While Loop:`**

  - Syntax :
           ```bash
             do {
               // Code to be executed
             } while (condition);
               ```

   - Example :
           ```js
           let i = 0;
           do {
               console.log(i);
               i++;
           } while (i < 5);
           ```


4. **`For Each Loop (using `for...of`):`**

  - Syntax :
           ```bash
           for (const element of iterable) {
            // Code to be executed in each iteration
            }
            ```

   - Example :
           ```js
            const numbers = [1, 2, 3, 4, 5];
             for (const num of numbers) {
                 console.log(num);
             }
             ```


5. **`For-In Loop (for objects):`**

  - Syntax :
           ```bash
           for (const key in object) {
            // Code to be executed in each iteration
            }
            ```

   - Example :
           ```js
          const person = { name: 'John', age: 30, job: 'developer' };
           for (const key in person) {
               console.log(key, person[key]);
           }
           ```