<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
# <span>Skill Up:</span> <span>Code</span>



<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/atom-intro.ogg" -->
## Atom Editor
![Atom editor](images/Atom_editor_logo.svg)

Note:
For this course we're going to use Atom. There are a lot of different text editors available and lots are people are pretty dedicated to their favourite. If you already have a favourite feel free to use that. But for those getting starting we recommend using atom


<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/atom-why.ogg" -->
### Why use atom
* Cross platform
* Configurable (HTML & CSS)
* Easy to setup and learn
* Package manager
* Cool features
	* Syntax highlighting
	* Smart autocomplete
	* Search and browse project files
	* Git integration

Note:
Atom is a cross platform, customisable text editor for coding. It is easy to setup and get started with but lets you complately configure the look and feel using HTML and CSS and to extend the functionality with plugins. It also comes with a lot of useful features out of the box like autocomplete, syntax highlighting and project wide search.
It is also really customisable using web languages. You can change the whole application theming using just CSS!


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
<video>
	<source data-src="videos/atom-intro.webm " type="video/webm" />
</video>


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Atom: Activity
* Open atom and add the document you made before class as a project
* Explore atom features
	* Open settings menu (ctl+,)
	* Explore features in the command palette (ctl+shift+p)
	* Explore keyboard shortcuts from a list like [https://github.com/nwinkler/atom-keyboard-shortcuts](https://github.com/nwinkler/atom-keyboard-shortcuts)


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
Share what you found


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Atom plugins
* Open the settings menu (ctl+,) and select install
* Type in devdocs and install the package
* Now go to your html document and select a tag name
* Press ctl+alt+D to open the documentation for that tag from [https://devdocs.io](devdocs.io)



<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
## Git


<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/git-what.ogg" -->
### What is git
* Source control
* Version control
* Distributed

Note:
Git is a distributed source and version control platform. It tracks changes to our files and stores those changes on a server.


<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/git-why.ogg" -->
### Why use git
* Store and share source code
* Tracks changes and versions over time
	* Can go back if we broke something
* Allows multiple people to work on the same code without disrupting eachother

Note:
Tracking our code changes on git makes it easy to share and prevents us from trying to manage multiple versions when we're trying something new. If you broke something, you can just go revert your code back to an earlier state. Because it stores changes, instead of the whole file, it also makes it easier for multiple people to work on the same code without breaking eachother's work.


<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/git-functions.ogg" -->
### Git functions
* Clone - Copy a repository to our local machine
* Add - Stage a file to commit
* Commit - Store a code change in git
* Push - send our code changes to the server
* Fetch - Get code from the server
* Merge - Mix new code in with ours or vice versa
* Rebase - Like merge but different

Note:
This are some common git functions. Don't worry, you don't need to learn them all now. You might also hear git pull. This is a shortcut command to fetch and merge


<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/git-github.ogg" -->
### Github
* A public git server
* A place to publish and share your code
* A place to find and download code other people have written
* A platform to submit code changes to open source projects

Note:
Github is a public git server. We're going to use it in this course to track our projects. It is a public place to publish and share your code. IT is also a great place to find and download code that other people have written. It's also great to share on your CV as it shows what you can do.


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Activity: Setup a git repository
* Register for github
* Create a new repository for your prep for unit


<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/git-wingit.ogg" -->
### WinGit client
* Lots of clients available
* Download from [https://git-scm.com/](https://git-scm.com/)
* GUI with Git GUI and command prompt with Git Bash

Note:
There are a lot of git clients about. For those of you on windows, I'd suggest using Git GUI for windows or the git client built in to Atom


<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/git-clone.ogg" -->
#### Clone a repository
![Git GUI open menu with "Git GUI here" highlighted](images/gitgui-open.png) <!-- .element: class="screenshot-small fragment current-visible" data-fragment-index="1" -->
![Git GUI new repoitory and clone options](images/gitgui-menu-new.png) <!-- .element: class="screenshot-small fragment current-visible" data-fragment-index="2" -->
![Git GUI clone menu](images/gitgui-menu-clone.png) <!-- .element: class="screenshot-small fragment current-visible" data-fragment-index="3" -->

Note:
To clone an existing repository to your computer, right click where you want to clone it and select "Git GUI here". Select "Clone existing repository" and enter the git address in "Source Location". Enter the path you want to clone to in "Target directory". Note that the final directory in target directory should not exist as git will create it for you.


<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/git-merge.ogg" -->
#### Fetch changes
![Git GUI remote menu](images/gitgui-fetch.png) <!-- .element: class="fragment" data-fragment-index="1" -->
![Git GUI merge menu](images/gitgui-merge.png) <!-- .element: class="fragment" data-fragment-index="2" -->

Note:
To get the latests changes from the server open Git GUI, select "Remote" from the menu, "Fetch from" then "origin". This downloads the latests changes from the server. To mix the changes in with your code select the "Merge" menu then "Local merge". Now your code is up to date.


<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/git-commit.ogg" -->
### Commit and Push
![Git GUI buttons with rescan highlighted](images/gitgui-rescan.png) <!-- .element: class="fragment" data-fragment-index="1" -->
![Git GUI commit menu with stage selected](images/gitgui-stage.png) <!-- .element: class="fragment" data-fragment-index="2" -->
![Git GUI buttons with commit selected](images/gitgui-commit.png) <!-- .element: class="fragment" data-fragment-index="3" -->
![Git GUI buttons with push selected](images/gitgui-push.png) <!-- .element: class="fragment" data-fragment-index="4" -->

Note:
When you finish you'll need to commit to save your work and push to send them to the server. From Git GUI select "rescan" to search for changed files. You should see a list of modified files appear. Now open the Commit menu and select "Stage to commit". Now your files are staged you can commit them to the repository. Enter a description of what has changed in the "Commit Message" field and click the "commit button". Your changes are now saved". Click the push button to send your changes to the server.


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Activity: Git local repository
* Clone your repository to your local machine
	* You can get the address from the green clone button on github
* Copy your prep for unit site to the directory
* Add the new files to git
* Commit the staged files with the comment "add initial files"
* Push your code and check it appears on the github website


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Some tips
* Fetch from the server before you start writing
* Push whenever you finish writing
* A commit should be self-contained
	* If you are editing multiple files, include them all
	* Keep them small so it is easy to see what has changed
	* It is better to commit too frequently rather than not enough
	* Try not to break things



<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
## HTML Validation


<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/validate-why.ogg" -->
### Why validate
* Identify mistakes
	* Typos
	* Unclosed tags
	* Missing doctype
	* Weird stuff

Note:
If you make a mistake in your HTML the browser will guess what you were trying to do and show that. This means that sometimes you don’t notice if you forgot to close a tag or used an invalid property. Unfortunately, because the browsers guess what they think you’re trying to do it might not be what you intended and might not work the same in all browsers. To address this we can validate our HTML.


<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/validate-demo.ogg" -->
<video>
	<source data-src="videos/html-validator.webm" type="video/webm" />
</video>

Note:
Here I'm validating my HTML using the W3C validator. You can see I've made some mistakes. I accidently included an extra < in an img tag and forgot to close some tags


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Validation Exercise
* Visit [https://validator.w3.org/](https://validator.w3.org/)
* Validate your page by direct input
* Fix any issues you can
* Commit you changes to github with a meaningful commit message
* Discuss what you found



<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/semantic-intro.ogg" -->
## Semantic HTML
* HTML describes the structure of the page <!-- .element: class="fragment" data-fragment-index="1" -->
* Semantic HTML adds meanining <!-- .element: class="fragment" data-fragment-index="1" -->
* Not about look and feel <!-- .element: class="fragment" data-fragment-index="1" -->

Note:
HTML represents the content and structure of a page. We spend so much time thinking about what the page looks like that we sometimes forget this. But when writing HTML we shouldn’t be thinking about the visual layout so much as the structural layout.


<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/semantic-why.ogg" -->
### Why do semantics matter
* Bots and SEO
* Vision impaired users
* People with arthritis
* Someone eating a sandwich
* Developers picking up your code (you)

Note:
Not everyone looks at a page as we see it rendered. Just as not everyone navigates it with a keyboard and a mouse. A well structured page pages it easier to parse and navigate for all users. Some examples of users we might want to consider.


<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/semantic-elements-old.ogg" -->
### Semantic elements
Describe what is in the tag
* form
* img
* table
* ul

Note:
Semantic elements describe what sort of data is in the element. Some you might have seen include the form element, which says this is an input form, the image element which describes an image, table elements which tell us we're looking at tabular data and a ul element which describes a list of items where the order does not matter.


<!-- .slide: data-background-image="images/bg-mouse.jpg" data-audio-src="audio/semantic-elements-html5.ogg" -->
### New HTML5 semantic elements
* header
* main
* footer
* nav
* section
* article

Note:
HTML5 bought us a lot of new semantic elements. The big changes are the structural elements that tells us where the content belongs in the page structure. What do you think these mean?


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Semantics Activity
* Have a look at the element list at [https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_categories#Flow_content](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_categories#Flow_content)
* Look at the flowchart at [http://html5doctor.com/downloads/h5d-sectioning-flowchart.png](http://html5doctor.com/downloads/h5d-sectioning-flowchart.png)
* Update your HTML to use the new semantic elements


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Questions
* When do you think you should use a div element?
* How should you name a new section?
* What do you think about the new semantic elements?
	* Too many
	* Not enouch
	* Too confusing?


<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
### Final thoughs
<blockquote cite="http://html5doctor.com/lets-talk-about-semantics/">
	<p>Don&#39;t think of &lt;article&gt; as a magazine article. Think of it as an article of clothing, an independent entity that can be arranged in conjunction with other articles of clothing, but is a complete thing in itself.</p>
	<footer><a href="http://html5doctor.com/lets-talk-about-semantics/">Bruce Lawson</a></footer>
</blockquote>



<!-- .slide: data-background-image="images/bg-mouse.jpg" -->
## Final Activity
* Update your site to include semantic elements
* Commit your changes to git with the message "Use semantic elements"
* Run your code through the [W3C validator](https://validator.w3.org/) again
