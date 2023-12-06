# SOLUTION

## Conditional Statements
  Conditional statements are programming constructs that allow the execution of different code blocks based on whether a specified condition evaluates to true or false. These statements enable the development of more flexible and dynamic programs by controlling the flow of execution based on certain criteria.

## Different Conditional Statements

1. **If Statement:**

  - Syntax :
           ```bash
           if (condition) {
               // Code block to be executed if the condition is true
              }
           ```

   - Example :
           ```js
           let x = 19;

            if (x > 10) {
             console.log('x is greater than 10');
             }
          ```

         
2. **If-Else Statement:**

  - Syntax :
           ```bash
           if (condition) {
               // Code block to be executed if the condition is true
              }else {
               // Code block to be executed if the condition is false
             }
           ```

   - Example :
          ```js
            let y = 3;

             if (y % 2 === 0) {
             console.log('y is an even number');
            } else {
             console.log('y is an odd number');
             }
          ```


3. **If Statement:**

  - Syntax :
         ```bash
           if (condition1) {
              // Code block to be executed if condition1 is true
           } else if (condition2) {
             // Code block to be executed if condition2 is true
           } else {
             // Code block to be executed if none of the conditions are true
           }
        ```

   - Example :
           ```js
           let temp = 5;

           if (temp <= 20) {
             console.log('Weather is cold');
           } else if (temp > 20 && temp < 30) {
             console.log('Weather is normal');
           } else {
             console.log('Weather is hot');
           }
          ```


4. **Switch Statement:**

  - Syntax :
           ```bash
           switch (expression) {
              case value1:
                // Code block to be executed if expression is equal to value1
                break;
              case value2:
                // Code block to be executed if expression is equal to value2
                break;
              // Additional cases as needed
              default:
                // Code block to be executed if expression doesn't match any case
        }

           ```

   - Example :
           ```js
            let day = 'Monday';

             switch (day) {
               case 'Monday':
                 console.log('Its the start of the week.');
                 break;
               case 'Friday':
                 console.log('Its almost the weekend!');
                 break;
               default:
                 console.log('Its a regular day.');
             }

          ```