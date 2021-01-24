# javascript-for-loops

JavaScript `for` loops allow code to repeat a block of code. A typical `for` loop has the following structure:

```javascript
for(define a counter variable; condition; increment)
{
  // Code to repeat as long as the condition is true
}
```

The code in between the open `(` and close `)` contains three pieces:

1. Define a counter variable. This part of the `for` loop is executed once before the first iteration of the loop. This variable will be used to track which iteration the loop is currently executing. Typically this code creates a new variable (often called `i`) and sets it to zero. 
2. Define a condition. This part of the `for` loop is checked once before each iteration of the loop. This condition is structured much like a condition in an `if` statement. The loop will continue repeating as long as the condition is true. 
3. Set the increment. This part of the `for` loop is executed once after each iteration of the loop. This statement determines how the counter variable (defined in the first part of teh `for` loop) is changed each time the loop repeats. 

For example, the folloing loop will repeat five times:

``javascript
for(var i = 0; i < 5; i ++)
{
  // Code to repeat as long as the condition is true
}
```
