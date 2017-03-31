# Module 1 Review Questions and Exercises

## Instructions

1. Click "edit" at the top of the page.
2. Fill in your answers below each question.
3. Save your changes and send a link to your mentor!

## HTML

### Questions

1. What is HTML and what is it used for?
HyperText Mark-up Language is used to mark-up a document to specify attributes, links, fonts, images, etc.
2. What is the difference between an ID and a class?
ID can only be used in one element, class can be used multiple times
3. What does it mean to write "semantic" HTML?
to write code with meaning

### Exercises

1. Write a paragraph tag with a class of "highlight" and content "Watch out!".
<p> <div class highlight = "Watch out!"> </p>

2. Write an HTML image tag to show an image called `profile-picture.jpg`.
<img src="profile-picture.jpg"> 

3. Write a link tag that links to http://google.com.
<a href="http://google.com"> </a>

5. Write an complete standard HTML document outline (including a DOCTYPE, and `<html>`, `<head>`, and `<body>` tags).
<!DOCTYPE html>
  <head>
  </head>
  <body>
  </body>
</html>

6. Inside of the code for the previous exercise, write the appropriate tag to link to a script file called `main.js`
<!DOCTYPE html>
<head>
</head>
<body>
<script src="main.js">></script>
</body>
</html>
7. Inside of the code for the previous exercise, write the appropriate tag to link to a stylesheet file called `main.css`.
<!DOCTYPE html>
  <head>
  </head>
  <body>
    <script src="main.js">></script>
    <link rel="stylesheet" href="main.css>
  </body>
</html>

8. Write a numbered list in HTML and list three of your favorite books.
<ol>
  <li>Game Plan</li>
  <li>Essential Oils</li>
  <li>Gone with the Wind</li>
</ol>

9. Fix the indentation of the following HTML sample:

  ```html
<div>
    <ul>
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
    </ul>
 </div>
  ```

## CSS

### Questions

1. What is CSS and what is it used for?
Cascading Style Sheets is used to change the appearance of HTML

2. What is the CSS box model?
is an invisible box that wraps up everything in html

3. What's the difference between margin and padding?
padding is outside the content, and margin is the most outer box outside the border


### Exercises

1. Write a CSS rule to make the text of all `h1` tags red.

h { text-color: red;}

2. Write a CSS rule to make the background color of the link with `class="btn"` blue:

  ```html
  <a href="#" class="btn">Learn more</a>
  ```
  
  class:btn { background-color: blue;}
  

3. Write a CSS rule to give the first paragraph in the following HTML a font size of `20px`, but not the second paragraph.

  ```html
  <header class="jumbotron">
    <p>Hello, World!</p>
  </header>

  <p>Welcome to this awesome website!</p>
  ```

p:parent { font: 20px;}

## JavaScript

### Questions

1. What is a function? What are they used for?
is a block of code to perform a specific task.

2. What is the difference between `==` and `===`?
the == will return an equal value, === will return an equal value & equal type

3. What is the difference between global and local scope variables?
local is the variable that is within the function, global goes beyond the local information assigned outside the function

4. What is a boolean value?
is a value that is true or false

5. What is an array?
is multiple values 

### Exercises

1. Write a line that declares a variable called `myName` and set its value to your name.
var myName = "Edna";

2. Write a loop that logs the numbers 1 through 10 to the console.
for (var number = 1; number <= 10; number++) {
console.log(number);
}

3. Translate the following pseudocode into JavaScript: if `score` is greater than `3` and `lives` is greater than `0`, alert "You win!".
if (score > 3 && lives > 0) {
alert ("You win!");
}

4. Write a function `sayHello` that takes one argument, a name, and logs "Hello, <name>!" to the console. Then, call the function below the function definition and pass in your name as the argument.
function sayHello(name) {
console.log("Hello, " + name + "!");
}
sayHello("Edna");

5. What would the following script log to the console?

  ```javascript
  var currentSong = "Call Me Maybe";

  function setSong(song) {
    currentSong = song;
  }

  setSong("Friday, Friday");

  console.log(currentSong);
  ```
"Friday, Friday"


6. What would the following script log to the console?

  ```javascript
  var add = function(a, b) {
    return a + b;
  }

  var result = add(3, 7);

  console.log(result);
  ```
 10
 
7. What would the following script log to the console?

  ```javascript
  var helloGoodbye = function(name) {
    return sayHello(name) + " " + sayGoodbye(name);
  }

  var sayHello = function(name) {
    return "Hello " + name " !";
  }

  var sayGoodbye = function(name) {
    return "Goodbye " + name " !";
  }

  console.log(helloGoodbye("Sarah"));
  ```
Goodbye Sarah !

8. Write a function `findLongestWord()` that takes an array of words and returns the length of the longest one.

function findLongestWord(array) {
  for (var i = 0; i < array.length; i++) {
   if (array[i].length > array);
  }
    return array[i].lenght;
}


9. Define a function `sum()` that sums all the numbers in an array of numbers. For example, `sum([1,2,3,4])` should return 10.

function sum () {
    for (var i = 0; array.length; i++) {
     sum += array.length[i];
}
 return sum;
}

10. Write a function that takes a character (i.e. a string of length 1) and returns true if it is a vowel, false otherwise.

function character () {
  if ( charAt(1) == vowel) {
    return true;
}
  else {
    return false;
}

11. Write the correct line to make `"Woof!"` show up in the console based on this script:

  ```javascript
  var pet = {
    name: "Charles",
    goodDog: true,
    speak: function() {
    if (name + goodDog == "Charles" + true);
      console.log("Woof!");
    }
  };
  ```
  

12. Using the same script as above, write the correct line to log the dog's name to the console.

console.log(name);

## Command Line

### Questions

1. What is the command line and what is it used for?
is used to perform the task assigned

2. What does the command `ls` do?
lists the files 

3. What does the command `pwd` do?
print working directory
4. What does the following command do: `cd my-cool-project`
changes directory to my-cool-project

### Exercises

1. Write the command to make a new directory called "my-cool-project".
mkdir my-cool-project

2. Write the command to create a file called "index.html".
touch index.html

3. Write the command to delete a file called "main.css".
git rm  main.css
## Git

### Questions

1. What is Git and what is it used for? 
Distributed Version Control System is used to manage repositories

2. What's the difference between a local repository and a remote repository?
local is your private repository and is stored locally, remote is stored in a different server most likely public.

### Exercises

1. Write the command that you would use to create a new local Git repository.
git init new

2. Write the command to stage a file called `index.html` to be committed.
git stage index.html commit -m
3. Write the command to view the current status of the git repository.
git status
