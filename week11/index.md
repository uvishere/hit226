<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
# Lets Code



<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## Device testing
You don't always have multiple devices on which to test your site but there are some ways we can do the next best thing.


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Inside of Chrome

You can also simulate devices right inside of Chrome, read through the Google Developers article on Chrome Device Mode

https://developers.google.com/web/tools/chrome-devtools/device-mode/ 


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Mobile testing websites

Upload your page/s to GitHub pages first and then use the URL to the page when testing.

* [Mobile Test](http://mobiletest.me/)
* [Mobile Phone Emulator](http://www.mobilephoneemulator.com/)
* [Google's Mobile-Friendly Test](https://search.google.com/test/mobile-friendly)


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Remote debugging on real devices

* [Android](https://developers.google.com/web/tools/chrome-devtools/debug/remote-debugging/remote-debugging?hl=en)
* [iPhone](http://moduscreate.com/enable-remote-web-inspector-in-ios-6/)



<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## Finishing up


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Make a checklist
* Create a checklist of things you need to deliver
* Before handing your project over go through your checklist
* Is there anything you forgot to double check?


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
#### Example checklist
* Is your spelling and grammar correct
* Does your website validate
* Does it adhere to best practices
* Make sure there are no broken links
* Do all images work?


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Have a finishing meeting
* Get together and discuss what you need to do
* Is anything missing?
* Has everyone finished their part?


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Review your documentation
You might not look at your project again for a while. But what if you have to pick it up in a year?

Ensure your documentation tells you
* Where do you find resources?
* What guidelines does the project follow?
* Does the project have any dependencies?
	* e.g. external resources


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Walk through the hosted website
* Sometimes things change when you deploy to the server
* Walk through your site and make sure it works
* Do this with your checklist
* Test on multiple devices


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Iterate so your product is ready to use
* Try and design and develop your MVPs so they are ready to go
* Test your MVP, design a new one and develop it
* You can do this forever but you can also stop any time


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Learn from the experience
* What lessons have you learned
* What went well?
* What didn't?
* What would you do the same or differenly


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### BONUS - jQuery
* fast and concise JavaScript library
* Released in 2006
* One of the most used JavaScript library
* simplifies HTML document traversing, event handling, animating, and Ajax interactions for Rapid Web Development.


### How to use??
1. Download local from [here](https://jquery.com/download/) and include it as a script
2. Use CDN
```html
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script> 
```


### How to start? 
* jQuery always start with $.()
* to reduce chances of error, always use:
```js
$(document).ready(function(){})
```


### Example
Hide a class/id/element
```js
	$(document).ready(function() {
		$(".myClass").hide();
	})
```
similary, you can show() the class too


### Useful functions
fadeIn() / fadeOut() / fadeToggle() - fade in/out/toggle a hidden element
```js  
//format is $(selector).fadeIn(speed,callback);
$("#div1").fadeIn("slow");
$("#div1").fadeOut();
$("#div3").fadeToggle(3000);
```


### useful functions
* after() - inserts content AFTER the selected HTML elements.
* before() - inserts content BEFORE the selected HTML elements.
* css() - sets or returns one or more style properties for the selected elements.


### Events
You can use DOM events (eg: click, keypress, mouseover, load, submit) and perform tasks based on that
```js
$("div").click( function () { 
   // do something here
});
```


### Try it yourself
Write a fuction using jQuery to change the color of the class "change-me"
```html
<html>
	<title> jQuery example </title>
	<body>
		<div class="change-me">
			<p> 
				Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.
			</p>
		</div>
</html>
```


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### All the best for your project