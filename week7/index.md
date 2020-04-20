<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
# <span>Skill Up:</span> <span>Code</span>



<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## Javascript Strings


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### What is a string
* A string is a representation of text
* Written using single quotes or double quotes

```js
'This is a string'
"This is also a string"
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Concatanting strings
You concatanate strings with the plus character

```js
var myString = 'this is a string.';
myString = myString + ' It is now a longer string.';
myString += ' You can also use the plus equals operator';
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Escaping special characters
If I use quotes to delimit a string how can I put a literal quote in my string?


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
Escape [special characters](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String#Escape_notation) with a backslash

* \' - Single quote
* \" - Double quote
* \\ - Backslash
* \n - new line

```js
var myString = 'That\'s my \"string\"';
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### HTML Special Characters
* Some characters mean special things in HTML (and URLs)
	* &amp;lt; : <
	* &amp;gt; : >
	* &amp;amp; : &
	* &amp;quot; : "
	* &amp;#39; : '
* Full lists are available online [http://www.degraeve.com/reference/specialcharacters.php](http://www.degraeve.com/reference/specialcharacters.php)


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### String properties and functions
* There are [lots of functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String#String_instances) to help probe and modify your strings


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### How long is my string
String.length

```js
if(inputString.length < 4) {
	throw new Error("Input string length is less than minimum length (4)");
}
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Get a character out of a string
You can use array notation for string characters

What does this output
```js
var myString = "this is a string";
console.log(myString[3]);
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Find a string inside a string
String.indexOf

What does this output?
```js
var catString = "I am going to talk about cats. Not catalogues but cats";
console.log(catString.indexOf('cat');
console.log(catStrring.indexOf('dog');
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Extract a string
String.slice(startIndex, endIndex)
* startIndex - the index to extracting from
* endIndex (optional) - The index to extract up to (not inluded in the extracted string)

What does this output?
```js
var catString = "I am going to talk about cats. Not catalogues but cats";
catString.slice(14, 18);
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Convert case
String.toUpperCase() and String.toLowerCase()

Useful for case insensitive checks
```js
if(input.value.toUpperCase() === name.toUpperCase()) {
	// input value matches name but may not be the same case
}
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Your turn
* Write a function that takes a string and converts the first character to upper case
* Can you make it convert the first letter of every sentance?


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Extra: Regular Expression Black Magic
* Regular expressions are too much to cover now but are extremly powerful.
* Like wildcard strings for programmers
* Take a while to learn but very useful

```js
var endNumber = testString.match(/(\d*)$/); // Get a number from the end of the string

if(input.value.match(/^[\d -]*$/)) {
	// Input value only contains numbers, spaces and hyphens
}
```





<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## Project structure


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Why the structure matters
* So you know where to put your code
* So you know where to find code
* So others know where to find code
* So others can modify your code


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### What do we have to save
* HTML documents
* CSS
* Javascript
* Images
* Documentation


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### A suggested structure
* There are many ways to structure your website
* This is just a guide


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### HTML Documents
* If there are only a few pages put them in the root directory
* If there is a complex site structure create directories for section


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
```
\
+-- contact.html
+-- index.html
+-- locations.html
```


<!-- .slide: class="fullscreen" data-background-image="../images/bg-mouse.jpg" -->
```
\
+-- locations
|   +-- darwin.html
|   +-- index.html
|   +-- katherine.html
|   +-- palmerston.html
+-- contact.html
+-- index.html
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### CSS files
* Put them in a styles or css directory
* Global CSS directory should be in the root directory
* Frameworks and libraries should be in a seperate external or lib directory
* For very large sites with multiple CSS files they should go under their relevant section
	* Nobody should have project sites this big


<!-- .slide: class="fullscreen" data-background-image="../images/bg-mouse.jpg" -->
```
\
+-- lib 
|   +-- bootstrap
|       +-- bootstrap.css
+-- locations
|   +-- darwin.html
|   +-- index.html
|   +-- katherine.html
|   +-- palmerston.html
+-- styles
|   +-- forms.css
|   +-- main.css
+-- contact.html
+-- index.html
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Javascript
* Javascript should go in a scripts directory
* External libraries should go in a seperate libs directory


<!-- .slide: class="fullscreen" data-background-image="../images/bg-mouse.jpg" -->
```
\
+-- lib 
|   +-- bootstrap
|   |   +-- bootstrap.css
|   |   +-- bootstrap.js
|   +-- jquery
|       +-- jquery.js 
+-- locations
+-- scripts
|   +-- form-validation.js
|   +-- main.js
+-- styles
+-- contact.html
+-- index.html
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Images
* Images should go in an images directory under the HTML file that requires them
* Global images should go in a directory under the root
* Remember images are referenced relative to the HTML or CSS file
* Images used in CSS may be placed in an images directory under the css


<!-- .slide: class="fullscreen" data-background-image="../images/bg-mouse.jpg" -->

```
\
+-- images
|   +-- logo.png
+-- lib 
+-- locations
|   +-- images
|   |   +-- darwin.jpg
|   |   +-- katherine.jpg
|   |   +-- palmerson.jpg
|   +-- darwin.html
|   +-- index.html
|   +-- katherine.html
|   +-- palmerston.html
+-- scripts
+-- styles
|   +-- images
|   |   +-- background.jpg
|   +-- forms.css
|   +-- main.css
+-- contact.html
+-- index.html
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Documentation
* Store any documentation you want to keep with your code in a seperate directory (except README.md)

```
\
+-- docs
|   +-- roles.docx
|   +-- sitemap.md
+-- images
+-- lib 
+-- locations
+-- scripts
+-- styles
+-- contact.html
+-- index.html
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Your turn
* What about reusable components or templates?



<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## Functions
* Follow along with your code editor <!-- .element class="fragment" data-fragment="1" -->


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### What are functions
* Reusable blocks of code
* They can take parameters
* They can return data


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
```js
/**
* Return the sum of two numbers
* @param {number} val1 The first value to get the sum of
* @param {number} val2 The second value to get the sum of
* @return {number} The sum of val1 and val2
**/
function sum(val1, val2) {
	return val1 + val2;
}
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Calling functions
* You call a function by passing the function name followed by brackets
* Parameters are passed in the brackets
* The function outputs the return value
```js
var mySum = sum(5, 4);
console.log(mySum);
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Your turn
* Write a function to calculate the factorial of a number
* It should take one number as the input
* It should return the product of the input value and all integers below it
* factorial(4) === 24 === 1 &#42; 2 &#42; 3 &#42; 4


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Variable scope
* Variables you declare inside a function *only* exist inside the function
* You can access variables that you created outside the function though


<!-- .slide: class="fullscreen" data-background-image="../images/bg-mouse.jpg" -->
```js
var extVal = 5;

function dummyFunc() {
	var funcVal = 4 + 5;
	console.log(funcVal); // 9
}

dummyFunc();
console.log(extVal); // 5
console.log(funcVal); // undefined
```



<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## Arrays


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### What is an array
* Store a sequence of data
* Store a series of values
* Can store any type of data
* Can even mix data (but you probably shouldn't)

```js
var vegetables = [
	'cucumber',
	'eggplant',
	'bean',
	'capscium'
];
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Accessing array data
* Access array values using square brackets and the item index
* Indexes start from 0
* You can also assign data to an index

```js
console.log(vegetables[0]); // cucumber
console.log(vegetables[4]); // undefined
vegetables[4] = 'pumpkin';
console.log(vegetables[4]); // pumpkin
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Finding the array length
* You can check how many elements are in an array with array.length
```js
console.log(vegetables.length); // 5
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Putting it together
```
for(var i = 0; i < vegetables.length; i++) {
	console.log(vegetables[i]);
}
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Some useful functions
* [indexOf(value)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/indexOf) get the index of a value if it exists in the array. Returns -1 if it does not exist
* [push(value)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/push) pushes the value onto the end of an array
* [pop()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/pop) Removes and returns the last value of an array
* [splice(pos, n, elem...)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice) Removes n number of items from the index pos. If elements are provided they are inserted at pos
* [join(seperator)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join) Returns all the elements of the array as a string. Inserts seperator if provided


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Lets code some code
Useful: You can also access the characters of a string like an array
* Write a JavaScript code to Display Characters from A to Z Using Loop. ``hint: use array``
* Write a JavaScript function to Check if the given character is Vowel or consonant? 
* Write a JavaScript program which accept a number as input and insert dashes (-) between each two even numbers. ``For example, if you accept 025468 the output should be 0-254-6-8``


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Lets code some code
* Write a JavaScript function to check if an email input is a valid email address? ``BONUS: Use Regular Expressions and test() method``
* Write a JavaScript program to find the most frequent item of an array.
```
Sample array: var arr1= [3, 'a', 'a', 'a', 2, 3, 'a', 3, 'a', 2, 4, 9, 3];
Sample Output: a (5 times)
```
