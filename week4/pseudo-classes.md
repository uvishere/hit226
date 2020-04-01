
<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## Pseudo Classes
* CSS can target elements based on state
	* Hovering over an item, clicking an item, a checkbox being ticked are all examples of state
* These are written using a colon, followed by the state.


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Pseudo class examples
* a:hover
	* anchor node which the user is hovering over with an input device
* .btn:active
	* A .btn which the user is clicking
* .gallery_item:nth-child(4)
	* The forth node which is a .gallery_item


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### More on pseudo classes
* State is useful for providing user feedback
* Also useful for styles which are specific to other conditions
	* Don't like the browsers default radio input appearance? .radio:checked will let you style it however you like
	* Need the last item in a collection of nodes to be styled differently? .item:last-child
* A full list can be found on [MDN](https://developer.mozilla.org/en/docs/Web/CSS/Pseudo-classes)


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Pseudo elements
* Not to be confused with pseudo-classes
* Forms part of the "shadow DOM"
* Creating a target to be styled that doesn't exist in the HTML
	* Helps us separate design and content
* Real-world use cases:
	* Adding extra items for styleing (such as transparent overlays, or anything else you can do with pure css)
	* Indicating a link is external


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### More pseudo elements
* Can not be targeted with JavaScript, so attaching events to them is not possible
* We target pseudo-elements is css using two colons
	* div::after – the after pseudo-element of all divs
* Special pseduo-elements: before and after
	* These can be targeted on any node that allows children, but must set a value for "content" in css for them to render.
* [MDN](https://developer.mozilla.org/en/docs/Web/CSS/Pseudo-elements) has a full reference on pseudo elements


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Task: Pseudo classes
* Download the Pseudo classes and elements folder from learnline or Github
	* https://github.com/HIT223/Week-2-Pseudo-Classes-and-Elements 
* Add styles to hover, focus, and active states for links
* Add labels to the headings with ::before, there are examples inside of label.css and typography.css of pseudo-element usage


