<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
# Lets Code



<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Prac 4 Feedback
<div class="column-wrapper">
	<div class="column">
		<img src="https://upload.wikimedia.org/wikipedia/commons/b/b6/Fxemoji_u1F601.svg" alt="smiley face" class="column-icon" />
		<ul class="happy-list">
			<li>Some great looking cards</li>
			<li>Some very informative git commit messages made it easy to see what people are doing</li>
			<li>Many people used the lighthouse tool to check accessibility</li>
			<li>Some very clever cards using things like clip-path and javascript</li>
		</ul>
	</div>
	<div class="column">
		<img src="https://upload.wikimedia.org/wikipedia/commons/4/41/Fxemoji_u1F622.svg" alt="sad face" class="column-icon" />
		<ul class="sad-list">
			<li>Looks like a lot of people are still using the web interface to delete and re-upload files.</li>
			<li>Many are not testing with lighthouse</li>
			<li>Only showing content on hover doesn&quot;t work with a keyboard or touchscreen</li>
			<li>Most teams didn&quot;t test their pages on mobile.</li>
		</ul>
	</div>
</div>


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## Marking guidelines
* Read the guidelines
	* If there are 15 marks for making it responsive - make sure you at least try
* Test your work before submitting
	* Does it validate?
	* How does it work when you resize the screen


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## Marking guidelines
* Make sure you submit correctly
	* Github pages
	* Use git commits to show your work



<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## General tips


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### No deprecated elements
* Use HTML for semantics and CSS for style

```html
<b>This is the wrong way to do bold</b>
<br>
<u>This is the wrong way to underline</u>
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Only underline links

```html
<a class="underline">I look just like a link</a>
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Put alt text in images
* An empty string does not count

```html
<img src="cat.jpg" alt="" />
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Do not use ID in CSS
* Use class instead. It is reusable

```css
#idElem {
	// bad
}

.class-elem {
	// good
}
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" data-transition="slide-in fade-out" -->
### Use a clear class naming system
* Underscores and hyphens are a great way to make class relationships clear

```css
.card {
	// general card style
}

.card__content {
	// Styling for the card content
}
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" data-transition="slide-in fade-out" -->
### Indent your HTML and CSS so it is easy to read
* I'll be happier when I mark and your employer won't get angry when they review your code

```html
<div>
<div>sometext</div>
<p>othertext</p>
<div>
<p>more text</p>
</div>
</div>
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" data-transition="fade-in slide-out" -->
### Indent your HTML and CSS so it is easy to read
* I'll be happier when I mark and your employer won't get angry when they review your code

```html
<div>
	<div>sometext</div>
	<p>othertext</p>
	<div>
		<p>more text</p>
	</div>
</div>
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Start with the smallest when going responsive
* Ensures your page will fit every screen size
* Use min-width in your media queries

```
@media(max-width: 800px) {
	// Try and fit everything into a smaller space
}

@media(min-width: 800px) {
	// Stretch out and use all the extra room
}
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## KeEP aN eYE on CASES
* Windows is not case sensitive
* Most web servers are
* Make sure you use the right case in filenames
* style.css != style.CSS



<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Review: ROT13
* Did anyone do the exercise from week 7?

```js
function rot13(string) {
  var alphabet = 'abcdefghijklmnopqrstuvwxyz'.split('');
  var letters = string.split('');
  var answer = '';
  var len = string.length
  for (i = 0; i !== len; i++) {
    var index = alphabet.indexOf(letters[i]);
    if (index >= 13) {
      index = index - 13;
      answer = answer + alphabet[index];
    } else {
      index = index + 13;
      answer = answer + alphabet[index];;
    }
  }
  console.log(answer);
}

rot13('abcdefghijklmnopqrstuvwxyz')
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Write a search function
* Can you get search working?
* [HIT226: Write a search function](https://codepen.io/elvey/pen/axedrW)



<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## Debugging


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Before we start
* Open the [hairsalon page](https://online.cdu.edu.au/bbcswebdav/xid-10170764_2) and attach the CSS file if it is not already
* Download and attach main.js
* What do you think this file is supposed to do?
* The file is broken, follow along with the debugger and see if you can find why


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### What is debugging
* Locating and fixing errors in code
* Performed at runtime
	* e.g. in the browser


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### How do we debug
* Chrome developer tools provides us with an _inline debugger_
* We can step through our code, line by line as it actually executes
* There are two main ways to do this


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Debugging from the sources tab
1. If you open up dev tools and go to sources you will find all your js files
2. Open the file you want to debug and find the function you want to troubleshoot
3. Find a line just before where you have a problem and click the line number
4. A blue arrow appears to indicate you have set a *break point*
5. When the code gets to your break point it will pause


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Open the debugger
<video>
	<source data-src="videos/debug-open.webm" type="video/webm" />
</video>


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Breakpoint
* Clicking on a line number creates a breakpoint
* When the code at the breakpoint is about to execute the browser will pause and open the deugger
* Lines with breakpoints are indicated with a blue arrow

![blue breakpoint marker](images/debug-breakpoint.png)


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Debug controls
* Play icon resumes normal code execution
* Step over continues to the next line in the current function
* Step into pauses on the first line of the function about to be executed
* Stop out pauses on the next line of the calling (parent) function
* Can you find out what the last two do?

![Debug control icons](images/debug-controls.png)


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Checking values
* You can hover your cursor over a variable to see the value it holds
* The scope pane shows all variables in the current scope
* You can add a variable to watch in the watch pane

![Debug scope name](images/debug-scope.png)


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
<video>
	<source data-src="videos/debug-breakpoint.webm" type="video/webm" />
</video>


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Review
* Why is main.js broken?
* Can you fix it?



<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## Accessing the DOM


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Querying Selectors

There are a bunch of ways to get elements from the DOM.

Two really stand out
* getElementById()
* getElementsByClassName()
* getElementsByTagName()
* querySelector() <!-- .element class="fragment fragment-em" data-fragment="1" -->
* querySelectorAll() <!-- .element class="fragment fragment-em" data-fragment="1" -->


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Query selectors
Use CSS selectors to get elements from the DOM

* querySelector() - Get the first matching element
* querySelectorAll() - Get a collection of elements

You can call them from document (the root of the DOM tree) or an element


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
```js
var btn = document
	.querySelector('#submitBtn');
console.log('submit button', btn);
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
```js
var inputs = document
	.querySelectorAll('.register-form input');
console.log('registration inputs', inputs);
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
<video>
	<source data-src="videos/devtools-query-dom.webm" type="video/webm" />
</video>


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Have a play
* Open index.html from hairsalon and type the following into the bottom of the console
	* document.querySelector('thumb')
	* document.querySelectorAll('thumb')
	* document.querySelectorAll('nav li')
	* document.querySelectorAll('nav > li')
	* document.querySelector('#logo')
	* document.querySelectorAll('#logo')


<!-- .slide: class="small-margin" data-background-image="../images/bg-mouse.jpg" -->
### Can you tell what this does?
```html
<form class="register-form">
	<label for="name">Name</label>
	<input id="name" name="name" />
	<label for="idCode">ID Code</label>
	<input id="idCode" name="id" />
</form>
```

```js
var inputs = document.querySelectorAll('.register-form input');
var registrationData = {};
for(var i = 0; i < inputs.length; i++) {
	var inputName = inputs[i].getAttribute('name');
	registrationData[inputName] = inputs[i].value;
}
```
