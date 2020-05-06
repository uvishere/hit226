<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
# Lets Code


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## Prac 4 grades

* 80 - 100	10
* 70 - 79	13
* 60 - 69	11
* 50 - 59	9
* 0 - 49	15



<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## Classes and javascript
* Classlist lets you add/remove/check classes on elements


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Add a class
```js
document.querySelector('#registerForm')
	.classList.add('focus');
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Remove a class
```js
document.querySelector('#registerForm')
	.classList.remove('focus');
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Check for a class
```js
var registerForm = document.querySelector('#registerForm');
if(registerForm.classList.contains('active')) {
	console.log('Register form is active');
}
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Toggle a class on or off
```js
document.querySelector('#registerForm')
	.classList.toggle('focus');
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Your turn
* Use classList to hide/show extra text
* Activity on [codepen](https://codepen.io/elvey/pen/VOeMBv)

```js
/**
* Event handler when the read more button is clicked
* @param {Event} evt The click event
**/
function readMoreClicked(evt) {
	evt.preventDefault();
	// Add your code here
}

document.querySelector(;#readMoreBtn', readMoreClicked);
```



<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## Event Listeners


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
* An event listener is code that runs when a certain event happens
* Common events include
	* An element is clicked
	* An input is changed
	* Text is selected
	* Media is played or stopped


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Add an event listener
* assign event listener by calling `addEventListener` on the element
* Takes two arguments
	* Event to listen for
	* A callback

```js
var button = document.querySelector('#btn');
var btnClicked = function(evt) {
	console.log('Button clicked', evt);
});
button.addEventListener('click', btnClicked);
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### What's a callback???
* A callback is a function that is passed as a parameter to call later
* They are used to execute code after something happens
* We can pass the function like a variable or pass an anonymous function
	* An anonymous function is not saved anywhere

```js
var button = document.querySelector('#btn');
button.addEventListener('click', function(evt) {
	console.log('Button clicked', evt);
});
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Some events to listen to
* [mouseenter](https://developer.mozilla.org/en-US/docs/Web/Events/mouseenter)
* [mouseover](https://developer.mozilla.org/en-US/docs/Web/Events/mouseover)
* [mousemove](https://developer.mozilla.org/en-US/docs/Web/Events/mousemove)
* [mousedown](https://developer.mozilla.org/en-US/docs/Web/Events/mousedown)
* [mouseup](https://developer.mozilla.org/en-US/docs/Web/Events/mouseup)
* [click](https://developer.mozilla.org/en-US/docs/Web/Events/click)
* [wheel](https://developer.mozilla.org/en-US/docs/Web/Events/wheel)
* [mouseleave](https://developer.mozilla.org/en-US/docs/Web/Events/mouseleave)
* [mouseout](https://developer.mozilla.org/en-US/docs/Web/Events/mouseout)
* [select](https://developer.mozilla.org/en-US/docs/Web/Events/select)


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Try them out
[Mouse event demo](https://codepen.io/elvey/pen/gzPLxv)


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Remove an event listener
To remove an event listener you can call Element.removeEventListener() and pass it the event type and the function you want to remove.

```js
button.addEventListener('click', clickHandler);
button.removeEventListener('click', clickHandler);
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Code Challenge
Can you make a [drag and drop?](https://codepen.io/elvey/pen/ardLxo)


```js
/**
* Add drag and drop functionality to an element
* @param {Element} target The element to add drag and drop functions too
* @return {undefined} No return value
**/
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### A couple of gotchas
* Sometimes other actions can execute on events
	* Other event handlers
	* Browser default actions


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
#### Bubbles
* Some types of event &quot;bubble&quot; up the DOM tree
* This is also called Event Propagation
* This means that after an event fires on an element, it fires again on the parent
	* or before if we set them to &quot;capture&quot;
* We can prevent this with Event.stopPropagation()
* Try to only stop propagation when you have to. It can be really useful


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
#### Brower default handlers
* The browser has default actions for some events
* e.g. The browser redirects when a form is submitted or a link is clicked
* To prevent this all Event.preventDefault()


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Research further
* There are lots of different event types including
	* Network events
	* Focus events
	* CSS animation events
	* CSS transition events
	* View events
	* Keyboard events
	* Media events

Have a look at the [event types](https://developer.mozilla.org/en-US/docs/Web/Events) and see what you can do




<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## Editing the DOM


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Modifying attributions
You can read and set the properties of an element using dot notation

```js
var nameInput = document.querySelector('input[name="fname"]');
if(nameInput.value.toUpperCase === 'UV') {
	nameInput.value = 'uv';
}
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
You can access most attributes using dot notation

```js
var myInput = document.createElement('input');
myInput.id = 'nameInput';
myInput.className = 'fancy-input';
myInput.type = 'text';
myInput.required = true;
myInput.maxlength = '50';
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Modify the contents

innerHTML lets us set the HTML inside an element

```js
document.querySelector('section:first-child').innerHTML = 'hello';

document.querySelector('.hero').innerHTML
	= '<h3>Extra Bits</h3><p>There are lots of cool extra bits you can do with javascript</p>';
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Insert or move elements

Node.appendChild() will add an element to its children. If the element exists elsewhere it will be moved

```js
var newsletter = document.querySelector('.newsletter');
document.querySelector('.hero').appendChild(newsletter);
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Remove an element
Node.removeChild will remove an element from a node

```js
var newsletter = document.querySelector('.newsletter');
newsletter.parentElement.removeChild(newsletter);
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Create a new element
You can always create a new element using document.createElement

```js
var myNewDiv = document.createElement('div');
myNewDiv.innerHTML = '<h3>Cool stuff</h3><p>There is lots of cool stuff here but the best thing is that it is new!</p>';
document.querySelector('.hero').appendChild(myNewDiv);
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Your turn 1
* Download the [hair salon page](https://online.cdu.edu.au/courses/1/HIT226_Sem1_2019/db/_3159284_1/embedded/hairstylesalon-week8.zip)
* Hide all the paragraph text and Create Read more button.
* Only Display the paragraph when the button is clicked


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Your turn 2
* Finish the Drag and Drop code challenge
