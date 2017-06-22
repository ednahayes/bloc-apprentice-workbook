# Module 2 Review Questions and Exercises

## Instructions

1. Click "edit" at the top of the page.
2. Fill in your answers below each question.
3. Save your changes and send a link to your mentor!

*Note: any topics from the first assessment should be reviewed in addition to the questions below!*

## CSS

### Questions

1. What is the box model? 
is a css box model is the design & layout that wraps around HTML. It consist of content, padding, border and margin.

2. What is the difference between block and inline elements?

Block examples are structural elements, inline they are text-based.
Block elements begin in new lines, inline elements do not begin on new lines.

Block Takes up the full width available, with a new line before and after.

Inline Takes up only as much width as it needs, and does not force new lines 



3. What is responsive design?

Is designing websites responsive to their environment(screen size, layout, orientation)



4. Which selector is more specific, a tag selector or class selector?
class selector



5. What does `box-sizing` do?

is used to change the defaults Css Box model, which is used to calculate widths and heights of given elements.
it allows us to include the padding and border in an element's total width and height.



6. What's the difference between `relative` and `absolute` positioning?
An absolute positioned element can be placed anywhere in the page and is removed from the flow, it won't affect or be affected by any other element in the flow.  Relative positioning movs an element Relative to its original positioning.


### Exercises

1. Write a CSS rule to turn the background color of the link with the `.btn` class blue on hover:

  ```html
  <a href="#" class="btn">Learn more</a>
  ```
a.btn:hover {
  background-color: blue;
  }
  
  
2. Write a CSS rule to give the `.container` a maximum width of `980px` when the browser window is wider than `1200px`:

  ```html
  <div class="container">
    <h1>I'm a heading!</h1>
  </div>
  ```
  .container (min-width: 1200px)   {
  max-width: 980;
  }

3. Which text would be red in the following example?

  ```html
  <style>
    section p:last-child {
      color: red;
    }
  </style>

  <section>
    <p>First paragraph</p>
    <p>Second paragraph</p>
    <p>Third paragraph</p>
  </section>
  <section>
    <p>First paragraph</p>
    <p>Second paragraph</p>
    <p>Third paragraph</p>
  </section>
  ```

Third paragraph


4. Open this [JSBin](http://jsbin.com/qigiwuhepe/1/edit?html,css,output). Write a CSS rule using floats to make the HTML sample into a four column layout. Paste your udpated link below.


http://jsbin.com/canohej/edit?html,css,console,output

## JavaScript

### Questions

1. What is a callback?
IS when a function is called to be executed by a different function. 


### Exercises

1. Write a function `filterLongWords()` that takes an array of words and an integer `num` and returns the array of words that are longer than `num`.

function filterLongWords(array, int) {
  var list = " ";
  for (var i = 0; i<array.length; i++) {
     if (array[i].length > int) {
      list += array[i] + " ";
    }
  } return list;
}

console.log(filterLongWords(["list", "young", "to"], 3));


2. Write a function `charFreq()` that takes a string and builds a frequency listing of the characters contained in it. Represent the frequency listing as a Javascript object. Try it with something like `charFreq("abbabcbdbabdbdbabababcbcbab")`.

function charFreq(string) {
  var list = { }
  for (var i =0; i<string.length; i++) {
    var letter = string.charAt(i);
    if (letter in list) {
      list[letter] += +1;
    } else {
        list[letter] = 1;
      }
    
  } return list;
}

console.log(charFreq("abbabcbdbabdbdbabababcbcbab"));



## DOM Scripting

### Questions

1. What does DOM stand for and what is it?
Document Object Model is a standard for accessing documents.

### Exercises

1. Write a JavaScript statement that finds the element with the ID, `next`, and saves it to a variable called `nextButton`:

  ```html
  <a href="#" id="next" class="btn">Next</a>
  ```
 var nextButton = document.getElementByID('next');
  

2. Write another line that updates the text of `nextButton` to `"Next image"`.

document.getElementByID('nextButton').innerHTML = "Next image";


3. Write another line that adds a click event listener to `nextButton` so that when it's clicked the browser alerts `"Next image coming up."`.

nextButton.addEventListener("click", function() { alert("Next image coming up"); })


## jQuery

### Questions

1. What is a JavaScript library and why do we use them?
a collection of functions which are useful when writing web apps. Your code is in charge and it calls into the library when it sees fit.
IS a library of pre-written Javascript which allows for easier development of JavaScript-based applications. 
JavaScript libraries execute many common, time-consuming tasks that simplify development.


2. What is jQuery for?
 It makes things like HTML document traversal and manipulation, event handling, animation, and Ajax much simpler with an easy-to-use API that works across a multitude of browsers
 
 
### Exercises

1. Write a statement to select all elements with the `.btn` class using a jQuery selector and save them to a variable called `buttons`:

  ```html
  <a href="#" id="next" class="btn">Next</a>
  <a href="#" id="beginning" class="btn">Beginning</a>
  <a href="#" id="previous" class="btn">Previous</a>
  ```
var buttons = $('.btn')


2. Write another line that adds a click event to the buttons that logs `'click'` to the console when the button is clicked. Use the jQuery syntax.


$buttons.click(function (event) {
console.log("click")
}

## Angular

### Questions

1. How is a framework different than a library?
The framework is in charge and it calls into your code when it needs something app specific, a library Your code is in charge and it calls into the library when it sees fit

2. What is a controller? 
a Controller is defined by a JavaScript constructor function that is used to augment the Angular Scope. In the model-view-controller organization pattern, the controller contains the logic for interaction and behavior.

3. What is a view?
what the user sees (the DOM)

4. What is a single page application?
are Web apps that load a single HTML page and dynamically update that page as the user interacts with the app

5. What is a directive in Angular?
are extended HTML attributes with the prefix ng- . The ng-app directive initializes an AngularJS application. A directive is any extension to HTML provided by Angular.

## Git

### Exercises

1. Write a command to create a new branch called `bug-fix`.
git checkout -b bug-fix

2. If you're on the `master` branch, write a command to merge a branch called `bug-fix` into the `master` branch.
git merge bug-fix
