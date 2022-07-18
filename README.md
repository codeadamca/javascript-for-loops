# A Basic Introduction to JavaScript and For Loops

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

```javascript
for(var i = 0; i < 5; i ++)
{
  // Code to repeat as long as the condition is true
}
```

## Loops and Arrays

Combining loops with arrays makes displaying data from an array quite easy:

```javascript
var colours = new Array();
colours[0] = "Red";
colours[1] = "Blue";
colours[2] = "Green";

for(var i = 0; i < colours.length; i ++)
{
  document.write("<p>Colour number " + i + " is " + colours[i] + "</p>");
}
```

## Data

One of the most common coding tasks is iterating through a list of data and displaying the data using well formatted HTML. This could include lopping through a list of records from a MySQL database, looping through a JSON or XML document, or lopping through a list of data stored in an array. Here is a typical list of coding resources:

<table>
<tr><th>Name</th><th>URL</th><th>Description</th></tr>
<tr><td>W3Schools</td><td>http://www.w3schools.com/</td><td>W3Schools is a web developer information website, with tutorials and references relating to web development topics such as HTML, CSS, JavaScript and PHP.</td></tr>
<tr><td>Code Academy</td><td>https://www.codecademy.com/</td><td>Codecademy is an online interactive platform that offers free coding classes in 9 different programming languages.</td></tr>
<tr><td>W3</td><td>http://www.w3.org/</td><td>The World Wide Web Consortium is the main international standards organization for the World Wide Web.</td></tr>
</table>

Let's place this data in a JavaScript array:

```javascript
var links = [];

links[0] = {
  name: "W3Schools",
  url: "http://www.w3schools.com/",
  description: "W3Schools is a web developer information website, with tutorials and references relating to web development topics such as HTML, CSS, JavaScript and PHP."
};
links[1] = {
  name: "Code Academy",
  url: "https://www.codecademy.com/",
  description: "Codecademy is an online interactive platform that offers free coding classes in 9 different programming languages."
};

links[2] = {
  name: "W3",
  url: "http://www.w3.org/",
  description: "The World Wide Web Consortium is the main international standards organization for the World Wide Web."
}
```

Next, let's create a loop that runs once for each item in the `links` array:

```javascript
for(var i = 0; i < links.lengt; i ++)
{
}
```

And finally. in between the open `{` and close `}`, output the content from the array. Here is an example of a `document.write()` command outputting the link name:

```javascript
document.write("<h2>" + links[i]["name"] + "</h2>");
```

## Trying It Out

Continue adding code to the `for` loop so all of the content from the array is displayed using well formatted HTML.

## Tutorial Requirements:

* [Visual Studio Code](https://code.visualstudio.com/) or [Brackets](http://brackets.io/) (or any code editor)

Full tutorial URL: https://codeadam.ca/learning/javascript-for-loops.html

<a href="https://codeadam.ca">
<img src="https://codeadam.ca/images/code-block.png" width="100">
</a>
