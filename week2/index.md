<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
# <span>Skill Up:</span> <span>Code</span>


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
## What did you learn last week?
Without talking write down the top thing you learned last week



<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
## Structural elements

Note:
We talked last week about why semantic HTML is important. There are a lot of different elements. Lets have a look at a few. Don’t worry if you don’t remember them all, you can always come back to look later. 


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Headings

* 6 heading levels
	* &lt;h1&gt; ... &lt;h6&gt;
* Should be used in order
	* Do not skip heading types
* Usually only one h1 per page

Note:
HTML has 6 heading levels. H1 - h6 and should be used in order. A document should have exactly one h1 element and each heading should fall under the heading above it. Some guides say you shouldn't use anything more than h3 or h4, the headings exist for a reason and it is fine to use them but it might be a clue that your content is too complicated


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### &lt;nav&gt;
* Contains navigation links

Note:
Nav indicates that it contains navigation links. In your exercises last week quite a few people used nav elements which was really good to see. Please note that is is not a list element and may not have list items as direct children. It may however contain an ordered or more often, an unordered list.


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### &lt;figure&gt; and &lt;figcaption&gt;
* Image, diagram, graph, code snippet, etc...
* Self contained
* Use &lt;figcaption&gt; to add captions or legends

Note:
A figure is usually an image, diagram, graph, code snippet or similar. It should be self-contained and make sense without the surrounding content. Figcaption contains a caption or legend for the parent figure.


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### &lt;aside&gt;
* Only indirectly related to surrounding content
* Or related to core content but not part of the core content
* Like a sidebar or those sub-articles you sometimes see in a magazine


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### &lt;article&gt;
* Self contained content
* Would make sense without the rest of the page
* Should have a heading
* Can be nested
	* e.g. article for blog post and articles for comments

Note:
A self-contained item of content. It should generally have a heading. If you pulled an article out and put it on another page it should still make sense. Examples are blog posts, user comments or even items in an image gallery if they don’t need context. 


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### &lt;section&gt;
* Content that depends on the parent for context
* Would not make sense without surrounding content
* Should have a heading

Note:
An item of content that depends on the surrounding content for context. If you pulled a section out and put it elsewhere it would not make sense. A section should also generally have a heading. 


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### &lt;p&gt;
* Text paragraph

Note:
The paragraph tag should be used for all text paragraphs. This is preferable to a div as it is clear it contains a paragraph of text.


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### &lt;div&gt; and &lt;span&gt;
* Use for styling
* Has no impact on content structure

Note:
If a tag is needed for styling but should not have an impact on the structure of the context you should use a div or a span tag. 


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### &lt;input&gt;
* Not really structural
* Lots of new types with HTML5
	* email
	* date
	* number

Note:
Not really a structural element. But worth mentioning all the same. You are likely familiar with the input element. However HTML added a lot more types that give forms more semantic context. Instead of just text, radio, password, hidden, etc… We now have input types like email, date, number and tel. Note that these do not all give you a special input form but help advise the user’s browser what type of input is expected. For example tel is considered too complicated for browsers to validate but may prompt a mobile browser to first show a numeric keyboard.


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Activity: Write the markup
* [The importance of sections](https://www.smashingmagazine.com/2013/01/the-importance-of-sections/?_ga=2.72253905.354623181.1520469113-698638064.1518098509)
* [Content](https://online.cdu.edu.au/bbcswebdav/pid-2569075-dt-content-rid-8647604_2/xid-8647604_2)



<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
## GitHub Pages


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Free hosting for your repository


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### GitHub Settings
Open your GitHub settings by clicking the cog in the top menu bar
![GitHub menu bar showing settings on the left](images/github-settings.png)


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### GitHub Pages Settings
Scroll down to find the GitHub Pages section
![Settings for GitHub Pages before setup](images/github-settings-pages.png)


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Select a branch
Select the branch you want to publish and hit save
![Branch dialog for GitHub pages setup](images/github-settings-pages-dialog.png)


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### Pick a theme
Select the themes dialog and pick a theme to use. This theme will be used when your markdown is converted to HTML.
![Theme list when setting up GitHub pages](images/github-pages-themes.png)
Markdown is a great way to represent your project documentation.


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
### All done!
Pat yourself on the back and enjoy your website.
![Settings for GitHub pages after setup](images/github-settings-pages-complete.png)
It is a good idea to enforce HTTPS unless you have a specific need not to.



<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
## Browser and development tools



<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/browser-intro.ogg" -->
Plenty of good brower choices

![Firefox logo](images/Firefox_Logo,_2017.svg) <!-- .element: class="browser-icon" -->
![Google chrome logo](images/Google_Chrome_icon_2011.svg) <!-- .element: class="browser-icon" -->
![Microsoft edge logo](images/Microsoft_Edge_logo.svg) <!-- .element: class="browser-icon" -->

Note:
As you’re likely aware the different major browsers have some differences in the features they support and performance. Everyone has their own preferences and so in the workplace we need to test with all the major browsers.


<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/browser-chrome.ogg" -->
We're going to use chrome

![Disabled Firefox logo](images/Firefox_Logo,_2017.svg) <!-- .element: class="browser-icon browser-icon_disabled" -->
![Selected Google chrome logo](images/Google_Chrome_icon_2011.svg) <!-- .element: class="browser-icon browser-icon_selected" -->
![Disabled Microsoft edge logo](images/Microsoft_Edge_logo.svg) <!-- .element: class="browser-icon browser-icon_disabled" -->

* Modern feature set <!-- .element: class="fragment" data-fragment-index="1" -->
* Great development tools <!-- .element: class="fragment" data-fragment-index="1" -->

Note:
To make things simple, we’re just going to use Chrome for this class. Chrome has a very modern feature set and great development tools that will make our work much easier. Let’s get to know the features.



<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
## Chrome Lighthouse
<video>
	<source data-src="videos/lighthouse.webm " type="video/webm" />
</video>


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
## Test your site
* [Install Lighthouse](https://chrome.google.com/webstore/detail/lighthouse/blipmdconlkpinefehnmjammfjpmpbjk)
* Run lighthouse on your site from github pages
* [More details](https://developers.google.com/web/tools/lighthouse/)



<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
## Accessibility


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Tables
* Present tabular data
* Easy to scan by column or row
* Must be properly marked up for screen readers and other tools
* &lt;caption&gt; immediatly after &lt;table&gt;
* Headers should be marked `scope="col"` or `scope="row"`

Note:
Data tables are used to present tabular data. They are easy to sighted users to scan by column or row. They must be clearly marked up for tools like screen readers to read them properly. 
Captions are added immediately after the table is opened
Headers should be marked with scole=”col” or scope=”row”. This makes it clear if the header is for the row or column. 


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
#### Tables: Further reading
* [https://www.accessibility-developer-guide.com/examples/tables/](https://www.accessibility-developer-guide.com/examples/tables/)


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
```html
<table>
<caption>2018 Oscar Winders</caption>

<tr>
<th scope="col">Name</th>
<th scope="col">Category</th>
<th scope="col">Director</th>
</tr>

<tr>
<th scope="row">Guillermo del Toro</th>
<td>Best Picture</td>
<td>The Shape of Water</td>
</tr>

<tr>
<th scope="row">Get Out</th>
<td>Best original screenplay</td>
<td>Jordan Peele</td>
</tr>

</table>
```


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Forms
* Logical order
* Test with tab navigation
* Break large forms into groups with &lt;fieldset&gt;
* Input should always have a label
* Do not use placeholder instead of a label

Note:
Forms should be structured in a logical order. It is alright to change the order a little with styling (e.g. right to left or columns) but it should still be immediately intuitive which way the form flows. Try using tab to navigate the form to ensure it makes sense. Large forms should be broken into logical group using fieldsets. 
All inputs should have a label correctly attached using the for attribute. NEVER use placeholder instead of a label. Placeholder should be used to provide examples of expected input if the format is unclear.


<!-- .slide: data-background-image="../images/bg-mouse.jpg" -->
#### Form activity
* Fix the form on codepen
* [https://codepen.io/elvey/pen/OdePrM](https://codepen.io/elvey/pen/OdePrM)


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
#### Forms: Further reading
[https://www.accessibility-developer-guide.com/examples/forms/](https://www.accessibility-developer-guide.com/examples/forms/)


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Colour contrast
* Vision problems are incredibly common
* Red/green colour blindness affects ~8% of Northern European Men
* Strong contrast important for everyone

Note:
How many people wear glasses here?
Red green colour blindness affect 8% of Northern European Men (https://nei.nih.gov/health/color_blindness/facts_about) although it varies by ethnicity. 
Only around 1 in 100- eskimos are colour blind (http://www.colour-blindness.com/general/prevalence/)
Blue colour blindness is less common.
Strong contrast is not just for colourblind people though. It is hard for everyone to read with poor contrast and especially hard for people with failing vision.


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
![normal](images/vision-normal.png) <!-- .element: class="screenshot-small" -->
![deureranomaly](images/vision-deureranomaly.png) <!-- .element: class="screenshot-small fragment" data-fragment-index="1" -->
![deuteranopia](images/vision-deuteranopia.png) <!-- .element: class="screenshot-small fragment" data-fragment-index="1" -->
![protanopia](images/vision-protanopia.png) <!-- .element: class="screenshot-small fragment" data-fragment-index="1" -->
![tritanopia](images/vision-tritanopia.png) <!-- .element: class="screenshot-small fragment" data-fragment-index="1" -->
![monochrome](images/vision-monochrome.png) <!-- .element: class="screenshot-small fragment" data-fragment-index="1" -->


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
![blurry image](images/vision-blur.png)
* How many people need glasses? <!-- .element class="fragment" data-fragment-index="1" -->


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Activity: Fix the contrast
* Clone the repository from https://github.com/HIT226/lawfirm-exercise
* Fix colour contrast
	* Check using online tools
	* http://leaverou.github.io/contrast-ratio/


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Keyboard Navigation
* Must be possible to navigate without a mouse
* Try using tab
* Focus must be visible. Do not remove :focus styling
* Use correct elements to get default focus
* Can change focus with tabindex but be careful

Note:
Many users with mobility difficulties need to navigate without a mouse. You should be able to tab through the key elements of a page. It is also important to make it clear which elements are focused. 
Tabindex allows you to change tab focus. It can be useful but it is easy to screw up. It’s better to use the correct elements where possible.
:focus can help you show when an element is focused. You should not remove the browser default unless you are making it clearer.


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Media
* Videos should have subtitles
* Audio should have transcripts

Note:
Videos should have subtitles. Youtube offers same great predictive tools that help you get started making subtitles. Audio content should have a text transcript available.


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Images
* Use the alt tag!!!!!
* If the image doesn't add content use CSS
* Can caption diagrams using &lt;figure&gt; and &lt;figcaption&gt;

Note:
All content images require an alt tag to describe the image. If the image is not content it is usually better to include it using CSS. You can add captions using figure and figcaption. We'll talk about them later.


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/q_ATY9gimOM" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
