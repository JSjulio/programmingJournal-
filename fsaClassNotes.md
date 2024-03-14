# ZTM Web development 2023 Notes

In this Document I'll keep notes on the course. <br><br>

## How the Internet works

<!--
	todo                    How the internet works


*A Network is two or more devices connected through a wired or wireless connection

	• Network switch: Devices connect to network switches to allow for efficient connection.

	https://www.mapeditor.org/	Network switches then connect to other NS and this relationship creates the internet (eventually)

*Servers client relationship
		○  (or computers) provide us clients ,with websites, video streaming services, etc.

*ISP - Internet Service providers
        Allow for the server client relationship to exsist.
		○ Stored in a data center with other servers

*Data centers:
		○ physical Hardware which reflects the function of the server.
         (i.e: data storage might have a lot of data servers)
		○ Located all over the world.


	• Webservers
		○ Is a software that can: store website storage/admin, data storage, security, managin email etc.
		○ Web request
			§ Responding to million client web request per second.


	• Webpage vs Website
		○ Webpage is the a page that displays content in the browser.
		○ Website is a conenction a various web pages linked together.
			§ If all the webpages has the same address in the search bar, theyre probably under same website



	*Webpage breakdown
		○ At the most basic it’s a text document, however developers use sophisticated tools:

			§ Hyper text markup language:
				□  HTML: What you see  -> the foundation
				□ Uses mark up tags to create:
					® Headings, paragraphs, multimedia
                    □ Can be static
                    □ Or dynamic

			§ Cascading style sheets
			§ CSS: Colors and styles -> interior decoration
				□ Cascading style sheets : work by enhancing the HTML elements

			§ JavaScript: User interaction -> the business
				□ Programming language which has tools for
					® Interactivity, data processing, and control and action

	• Delivering the code occurs through Page Rendering:
		○ Lines of codes are proccessed in sequential order to show the page in the browser.



	• Browser: Software application used to surf the WWW (world wide web)
		○ Works by sending a request to a web server then receives the content
		○ Address is the URL : or Uniform Resource Locator
			§ The quest is made and the data text transfer protocol (HTTP is the form of communication between browser and the server)
			§ The browser then receives the content and displays it on the screen of my device.
			§
				□



	*How does a server request work in more detail:

		1. You open your browser , type in the domain name of the search engine. *ENTER**

		2. The webpage pings teh ISP , which pings the DNS (Domain Name Service)

         Webserver send a request back to the ISP which sends an IP address to the browser.

         Using the IP address we send that to the servers.

        The server sends back files to my personal computer to inlcude
            HMTL
            CSS
            JS

        When the browser recieves all the information, the page processes visually.



*Web Hosting : creating your own!
		○ Developers launch their own websites to the internet through this process.


-->

## Hosting options

<!--
*Hosting options

    *Shared hosting:
	    pay for a location on a webserver containing many other webhosting accounts
		○ You share the host website's
			§  processing power, memory, and bandwidth with other websites (slow)
		○ Cheap , good for small websites with a small number of visitors
		○ Used for practice by many developments
		○ Sometimes free but w/ limitations.


	*VPS hosting(virtual private servers)
		○ Physical server
		○ Dedicated: cpu, memory, and bandwidth BUT resources are fixed!
		○ More expensive


    *Dedicated hosting: Hardware server that is dedicated to just you.

	- Cloud hosting: allows for your website to be ran on a mixture of physical and virtual servers. IF the server fails your data stays online.
		○ You pay based on resource use. (i.eL if a file is transferred from the server to the client, and you pay for the bandwidth use for that download)



 -->

## HTML / HTML 5

 <!-- 

 *Rubber Duck Debugging
 Explaining a problem to a "duck" or innatimate object in order to ressolve a problem 

 *Stack Overflow 


<!-- 
?The anchoring other websites

*Relative path method:
Is used to link different data that within the same folder or location

	***Remember
	The file either has to be within the same folder(directory) 
	
	Or you have to specify the folder which it resides in: 
	 	i.e: <a href="test/index.html">Webpage1</a>
			    <!-- The "../" in link allows us to go back one directory"


*Absolute path 
Linking a non local website:
	<a href="https:....address">New Page</a>

*Linking an image: 
	 	<img src="google.com/335i" width> for inserting pictures

		?attribute: values that are enclosed within quotes, which adjust the behavior of the element. Above the attribute is the src. 



?HTML: Forms 

*See the Register form in ZTMWebsites for my first form(annotated with notes of coarse) 



?Annotating a File
Here I learned about 
-annotating a text,
-using tags like:
	-<div> block element which divides content for css styling purposes.
	-<span> inline element divider when using css

	? if im ever not sure on what type of element im using(inline / block) I can use inspector to find out. 



?HTML vs HTML 5

HTML was started in 1991 by Tim 

*HTML 5 is more modern. The difference is our modern web (HTML 5 ) 

	-accounts for phone pixel levels. 
	*has Semantic Elements

		i.e: 
		*Websites are more descriptive. Google uses "quolers" or a machine that reads the topic of your HTML , so it can then rank it in google. 

		So HTML 5 adds more meaning for the quolers so they're able to digest websites: 

			*Semantic Elements inlcude: 
				<h1>Register</h1>
				<nav>
					<a href="google.com">
				</nav>
				<footer> 
					<p>Website made with love</p>
				<footer>


? Copy a website: A useful tool!

	*Pressing opt+Command+U: 
	Allows us to view the source-> in many cases, the HTML of a website. 

		*Select all, copy and paste into a new file
		*You now have access the website you copied! 

-->

## CSS

<!--
						? Using CSS

*The head contains the Meta tags(the website title)
*and links that we need for the website


*Linking styles into websites:
	1.*Within the head under title:

		<Link href="css.style"> rel="stylesheet" type="text/css">


<br>
	2. You can switch the style an element withing the header or div elements with the style=" attribute inside an element

		<body>
			<header style="background-color: green;">

<br>

3. You can modify markup within the HTML using a <style> tag


			<style>
				li {
					background-color: purple;
				}
			</style>



-The CSS takes the last input it receives for a specific selector and applies that

-Inspect websites to see exactly how they were created.

-When creating a webpage of websites, in order to style differently I'm going to have to link different websites to different css pages
	-With that being said you should place more general modifications towards the top of the CSS file.

*Resources to use:
	CSS-tricks




todo 												CSS Selectors

*The order of css matters.
	Do note that the css arguments that are towards the bottom overide the top.
	?UNLESS it's a inline element.


*Main selectors include:

.class : is a less specific way to select an element
	<p class=webtext> -> .webtext
	<p class=webtext.active> -> .active
									*Would contain all of the .webtext css + more

#id : are the most specific way to select an element
	<div id="div1"> -> #div1


*
	* {
		This star encompasses all of the elements
	}


*element
	i.e: h2

*element, element
	Selects two elements

*id, class, element
	Selects two id, classes, or elements

*element(A) element(b)
	Selects only the second elements(b) that are in the first element


*element<div> > element <p>
	Select only (p) elements that are parents of the (div) element


*element(div) + element(p)
	Select and (p) element that is after and (div) element


*:hover
		h2 + p:hover{
				? the hover makes things dissappear until you hover over it
			color: black;
			text-align: center;
			border: 5px solid rgba(255, 176 170, 0.5);
			cursor: pointer
		}


*:last-child / :first-child
	Selects the last child or first child of whatever designated element
˜˜˜˜˜˜˜˜˜
		.webtext:last-child {
			border: 5px dashed green;
		}


*  !important (not reccomended)
	The important modifier overrides all the other css rules and prioritizes the one you " !important"-ed.

	? CSS concepts:

		Specificity
			You get specificity scores. The more specific something is, the more likely it will win out or retain a style.
				*the most specific being placing a style exactly within a section

		Importance
			see above.

		Source order
			The linked CSS that is in first place within the head take precedence.





todo 									Text Properties

There are several ways to alter the text on a website:


	text-decoration: underline/line-through;

	text-transform: uppercase/lowercase;

	line-hieght: 20px; <-- this is the space
	between sentences

	font-style: itallics;

	font-weight: 100-900; or bold

	font-size: 100% is base, 150% is bigger

	font-family: Georgia or "Times New Romen"..

			? seperated by a comma, then the second one is the secondary font, in the case the computer doesn't have the first font.




?              Using Google fonts:

1. Navigate to Google fonts, find a desired font, and press the "+"
2. Copy the link from the "+" into the head of your HTML file

3. add it to the CSS file into CSS file as shown on google.






todo						Modifying images in CSS

*Adding a img and using the wrap

1. Add, resize, and specify the alternate of the img <img>
	<img src="http://www.google.com/" width="200px" height="200px">

2.   In CSS the float property to wrap the text into the img

	img {
		float: left;
	}


3. In the HTML doc, under the img add a <footer>

	<footer>Website made with love</footer>

4.  To ensure that the footer doesn't wrap around the img , set the properties of the footer in CSS

	footer {
		clear: both;
		text-align: center;
	}



todo							The box model

	Is the model which considers the following dimensions


	1.Content
		Can be modified with "width" in CSS
			Width: 33px;
			hieght: 55px;



	2. Padding

		.boxmodel {
			padding: 5px(top), 20px(right), 5px(bottom) left(left)
			} // is the same thing as

			padding: 5px, 20px;

	3. Border

	4. Margins



todo 							px Vs em Vs rem

*Px:
Normal measurement, not in relation to anything.


*em:
This tags multiplies the size by the amount of the containing element. So if you have a <span> element within a <p> element and in CSS you place a rule saying

	span: 2em;

	Then the span is be twice as big as <p>'s size


*rem
Here the size "rem" is in relation to the root size of the HTML document



todo					Critical Rendering Path

*When your page is being loaded, the computer is attempting to render the page
	-What happens is it reaches out to a server and possibly
	-a google page (if you used google fonts,) to load the text.
		as a result, it takes longer to render your actual page.
		Long rendering times also happen when the CSS code is really long.


*CSS Minify : compresses the CSS you write, thus lowering bites, and shortening rendering times



todo 							Flexbox

flexbox is a tool used for programmers to organize the location of images on a website

Use link in Bookmarks to reference flexbox maneuvers

1. Get in the habit of building div containers that hold groups of images that you want to have a certain behavior in CSS


2. Assign the container display to flex:
	.container {
		display: flex
	}

3. If you want images to wrap around and stay in the width of a size changing webpage, then use Flex-wrap:

	.container {
		display: flex;
		flex-wrap: wrap;


4. In order to make the content centered in the container :

.container {
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
	}

5. Ensure to style the wording

	You can modify the font family / size
	Border, and ... DRUMMROLL! Width of the border!

		h1 {
		font-family: fantasy;
		font-size: 3em;
		border-bottom: 2px solid black;
		border-right: 2px solid black;
?		width: 400px;
		text-align: center;



todo								  CSS3


When implementing new properties use
W3Schools: CSS browser support reference IOT see if browser support the property.

Some properties like box-shadow (years back), were not supported on various browsers but said browsers has box-shadow in developemnt

You would have to use a browser prefix in order to implement that feature for said browser.

		normally:
		box-shadow: 4px 4px 5px #888888;

		isntead:
		-moz-box-shadow: 4px 4px 5px #888888;
		-ms-box-shadow: 4px 4px 5px #888888;
		-o-box-shadow:  4px 4px 5px #888888;
		etc.


? New tricks observed here:
*Modifying the body to margin 0 IOT align items left

*The transition(time) and transform(change) property:
	https://thoughtbot.com/blog/transitions-and-transforms for more information




todo 							      Responsive UI

* Responsive UI is that the website has features that allow it to adjust it's display for multiply device pixel sizes

	This made me think of something from Meta:
		 breakpoints which are indicated by infixes. Also think the CSS class-col rules that allow automatic adjustment of breakpoiints.


*Ques a Exercise: Assemble a Robot:

	position: relative;
		top: -120px;
		left: 90px;
?				other property values you can use are:
?				absolute| static | inherit | fixed | sticky
?		     https://css-tricks.com/almanac/properties/p/position/



*For this exercise I mainly used the code mentioned above in order to switch the position of an element.

*For some reason the
	?justify-content
property was not working? This was because I hadn't used the
*							flex: display;
property to place the items on the horizontal axis


*	I found this to be kind of ineffective because when I would enlarge the browser, the pieces of the robot would scatter.


todo 							        Bootstrap


*Bootstrap is a CSS / HTML Library that allows you to cut and paste different web features

Its as simple as copying the CSS / Javascript CDN (content delivery network) and placing it in the head or (for css) The bottom of the body (for javascript)).

* To add function into a website:

Go onto bootstrap, find the mod you want and copy/paste it into the body of the HTML
    -You will have to have the CSS / JS link in the body or the head.


*To modify the styling of the Boostrap additions:
	1. Create a CSS file and link it under the boostrap link in the <head>
	2. select the thing you want to change, and add a new CSS style




todo                                Boostrap 5 Update


*Updating Bootstrap:
to update versions go to bootstrap and copy the latest version (ensure to just copy the main directory to the URL)

i.e:
?<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.1/ (this is the portion you update)
dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-iYQeCzEYFbKj
A/T2uDLTpkwGzCiq6soy8tYaI1GyVh/UjpbCx/TYkiZhlZB6+fzT" crossorigin="anonymous">


todo                                Boostrap Grid

When boostrap first came out, it had a method to create a \
*Grid system.

Horizontally, columns had 12 lines that they could occupy.
This would be controlled by div class

<div class="col col-sm-6 col-md-12 col-lg-12>
The different modifiers (sm,md,lg) denote how big the window is.
The numbers to the right of the infixes denote how muuh of the twelve spaces the columns take at each modifier



todo                              Posting a Website






Todo 							   Using Animate.Css

You can either download the CSS file or link the file in the head of the HTML
Under *Other Exercises in ZTM Exercises, see how I used it.


todo                                 Creative Tim


*People Use Websites like creative Tim as a skeleton to create websites. They make mods to the index and CSS file template provided.

*Creative TimeIs a website that creates bootstrap themes using the BS toolkit. They have styles and custom actions as well

?                            Free HTML 5 / css templates:
Allow me to create a fast website without starting from the bottom see the following sites:

-mashup template



todo 								Understanding CSS Grid vs Flexbox vs Boostrap

It's good to use a combo Flexbox + CSS grid when creating a layout.

	*Flexbox: good at one demensional (i.e: columns)

	*CSS Grids: two demensional (columns and rows , like image galleries and portfolio projects)
		Is a newer feature compated to flexbox, so features have to be implemented manually for other browsers ..

		Honestly sounds like CSS GRids is King.

	Bootsrap4: Came before Flexbox and CSS grid. So it's outdated compared to the first two methods mentioned.




Todo 					   CSS GRID 1



*Steps to Creating a Grid System:
	1. You have to wrap all elements you want to Gird in <div class="container"> ..next give it them the CSS rule of:

	2. display of: Grid;

	3. Use the rules below to manipulate the size of the grid's pixels and the number of colums. In method

	*(a) a set pixel size of columns, and number of columsn

	*(b) I use percentages in order to take up more of the screen. This method still leaves space to scroll

	*(c) Fr value is the golden value to use when creating grids

		(a) grid-template-columns: 300px 300px 300px;
			tells your pages how many columns and what spacing
		(b) grid-template-columns: 25% 25% 25% 25%;
		(c) grid-template-columns: 1fr 1fr 1f2;
		?2 This value is relative, meaning you want three columns, where the last columns is twice the size of the first two

	4. Use grid gap IOT create a gap between all elements.
		grid-gap: 20px;


todo					CSS Grid 2

Rows can be defined as well
	*1. Grid-template-rows: 1fr 2fr;
		Any following rows will repeaet the same rule of previous rows .
	2.   grid-template-columns: repeat(3, 1fr);
			The first # is how many times you repeat
			The second # is what fr value you want repeated
	*3.   grid-template-columns: auto;
			Auto property automatically resizes to fit the content to its placement.



todo 					CSS Grid 3


*justify-items
 is a property that controls where within it's boxan elements starts at.

	Justify-items: stretch;
		Is the default for CSS Grid, where items are stretched along the row axis.



	justify-items: start;
		This aligns contents towards the start of the row.

	Justify-items: end;
		This algins contents towards the end the row in the grid system.

	align-items: start/end
		is the same as above but along the column axis. Here you can use


?Preferred methods of creating a grid layout

The instructors preferred method is derived from the style metioned below, however it allows for the website to be more responsive when using smaller pixel levels.
 *   grid-template-columns: repeat(3, 1fr);

Common grid patters:
 *	grid-template-columns: repeat(auto-fill, 300px)

Even better pattern:
	*grid-template-columns: repeat(auto-fill, minmax(200px, 1fr)
								how small columns are     max


todo                       CSS Grid 4



*Selecting Indivisual Items or Zones within the grid:
	In the example  we modify backgrounds of items by the background color:

 *Grid Column:

	.green {
		grid-column-start: 1;
		grid-column-end: 2; ->3;
	}
	?... if you change the end value to 3... Then you command for the zone to span from columns 1->3. This feature responsively changes with width of the page.

	shorthand version
	.green {
		grid-column-end: 1/3;
	}

	To make the zone spand all the way to the end:
	.green {
		grid-column-end: 1/-1;
	}

	If you're not too sure how many total grid you'll use:
	.green {
		grid-column-end: span 2;
	}


*Grid Row can also be used in a similar facet:

	grid-colum-end: 1/3
	grid-row: 1/3;




Todo 						CSS	GRID 5


Using Justify with Grid-column-end & Grid-row

	grid-colum-end: 1/3
	grid-row: 1/3;
	align-self: end;
		*This would take space of the selected grid, while also moving the green zone to the bottom Grid space.


Todo						CSS Layout

* Using all of skills I've learned up until now, create a layout for a website!
	The website must have a: Header, Cover, Project Grid, and Footer that is responsive.
	Use both Flexbox and CSS grid?




todo 							Creating a Layout


*New Things I Learned in this exercise:

? vh - or viewport hieght allows you to set a responsive height to containers. this value works in terms of percentages. 50vh means said container will take up 50% of the screen.

? Grid Wrapper - In the index document whenever you want to use CSS Grid create a Grid wrapper class
	<div class="zone blue grid-wapper">







 -->

# Full Stack Academy

 <!-- 

todo: 02 OCT 

*Vocabulary

sprint: when you're assigned to create a web feature in two weeks

react: created by Facebook. React allows for things to appear the way they do (think facebook, instagram, metaverse etc)

CRUD apps: a web app that has the function of creating, read, update, delete 


*Operating Systems 

MacOS and Linux are very similar in their communication with the computer system via the the terminal 

Windows is a whole different beast 



todo: 03 OCT

?: Overdue task Messing with Google assignment 
?: Learn how to use terminal within VSCode to commit things onto GITHUB

* Topics covered by michelle
	-HTML inspector tool: 
		You can use the inspector to play with elements, then copy paste into IDE 


	- box model 
	    to include: margin, borders, padding, 



	-inline / block elements 



	-basic HTML 



	-CSS Selectors
	

todo:  05OCT 

! ?: Overdue task Messing with Google assignment 


?: Commit documents to GitHub 
	1. Start by creating a repository in Github 
	2. Click the "Code" button and and copy the SSH link 
	3. IN VSC terminal, ensure that you're directory is in the correct folder you intend to modify 
	4. Clone the repo by running " git clone <SSH link>
	5. if prompted in terminal enter your password 
		

*Using the Command Line aka "terminal" 

*Command lines are essential because: 
-They allow us to connect to the cloud. We need to access a cloud in order
to deploy software. 
-In short it's the way modern software is deployed 
-Best way to be fast at computer 

*SSH key added to access Github ..... WHAT does this mean? 
	-With SSH keys, you can connect to GitHub without supplying your username and personal access token at each visit. You can also use an SSH key to sign commits. You can access and write data in repositories on GitHub.com using SSH (Secure Shell Protocol).



	? Command line inteface (CLI) lecture! 

	pwd -> ls -> cd FSA
	where am i -> where can i go -> change directory to FSA -> 


	*ls : list  all content in the current directory (folder) youre in
 	*cd : "change current directory 
	*pwd: shows the full path to current directory "where am I?" 
	*clear: cleans the terminal 
	*mkdir: make a directory 
	*cp: copy a file 
	*touch filename.txt creates a file 
	*mv: move a files 
	*cat READme: the cat shows whats available in the requsted file - READme in this case
	*rm: delete a file or folder. 
		rm -r (+the folder you want to delete) deletes the folder you want 
			-r: or 'recursive' is a flag that modifies the  the argument 
			argument: is the file / folder you want to use. 

			when you delete something with rm -r: you cannot get that file back! 

			!rm -rf.   NEVER use this. It deletes everything in your computer. 

init <filename
>


	*man + a command: gives you help on how to use a command. 

	npm run dev -- --host: find the live server for REACT 


	! TRY TO USE NANO
	*nano: edits a file , follow the information on the screen to navigate this command
	* cd ..     : means change directory up one level .... (..) essentially means back one folder 
	* cd ~ : brings you back home! 
	* sudo : gives you permission to complete whatever task 
	*tab - completes the type out in the command line 
	*the ^ arrow, copies the last line in the command line 
	*vim: AVOID using but in the case I do use it, use the : to escape this. 
	*vi: 


todo                                              09 OCT

*First twenty minutes of lesson: 
-discusses shortcuts:
	look up VsCode shortcuts 
-how to commit to Github from vscode 

?: GIT 

	*Git Commands
git remote -v : finds the remote url of a git project 

git add: starting tracking a file

git commit: adds a commit message to file(s)

git push: pushes the commited files to git
	   * git push --set-upstream origin (BranchName)
			This command pushes the branch that you made locally to GIThub
git status: shows the status of file(s)

git push origin main 

	git stash -> stashes the changes 
		pull the request from where you need them 
	git stash pop -> re renders the bag that you just commited 

	git rebase can be used instead of git merge 



*Understanding the Git -> GitHub process 
 

?	-Check Status 
		Use "git status" to see what bracnch I'm on and see what are the status of files that have not been commited ti Github just yet 

?	-STAGING 
		Use the "git add ." or "git add [Filename]" or git add my folder(replace my folder with folder path" to stage all changes or a specific change.

?	-Check Status 
		I should see there are changes ready to be commited 
			If I want to unstage a file: 
				"git reset HEAD example.html"
				
	
	-Deleting File
		If you delete a file you have to use git add to stage it OR use the command listed below to remove file and stage it. 
		"git rm example.html" 
		OR
		"git rm -r myfolder" 
				 (replace example.html with your file or folder name) 
			
?	-Commiting files 
		*when describing the change use active verbs to say what your code is doing, as sometimes commits are not approved.

		Use git commit -m "Descriptive message of commit" 

	-Git Status 
		if all changes have been committed and there are no untracked files it should say nothing to commit, working tree clean. 

	*unstage a commit: 

? Linking a Pre-existing project with a remote repo 

	*git remote add origin <repo link>
		To add an existing local project to a newly created remote repo: 
				 
					*or

	*git remote set-url origin <repo link> 
		If a remote repo is already set up and you want to change it: 

	*git push -u origin main 
		Make the first push request and 

		
			
*Some common unix commands:

ls: list all files and directories cd: change working directory cat: print output of file pwd: list current path of current working directory nano: edit file in nano editor touch: create empty file ssh-add: adds ssh key


*how to create branches
	branches are useful bc they allow for us to work on the main branch as a draft before committing. 


*Fork: 
	create a version of the original repo to allow you to make any changes you'd like. 


? class schedule is in Github: 
	https://github.com/FullstackAcademy/2310-fsa-et-web-pt-sf-class-repo



todo 							11 OCT 

*Today's lesson: fronted development 

?Key take aways:
-Before we learn Javascript and CSS we need good HTML! 
-elements just in their tag names should describe what they are (i.e: divs, )
-Semantics 
	-main/section dividers have inherent styling they come with (depending on the website)
	-examples are: header footer, article, section, table  .... etc 
		-Use MDN web docs semantics section for more information on everything semantics 
-Attributes: additional info added to element 
	-sizing, where an element will link to, styling options, and accessibility	
			-i.e: src anda alt 
				src: the link to an image 
				alt: you usually use this to describe what an image is 
*-when formatting: Ensure to have consistent indentations
-HTML tree is technically upside down, with the body being the 1st and the div or other syntax being the kids. 
-Use lowercase letters for elements and attributes 
-self closing tags, closed themselves within one tag. Often you'll see them in the header with the exception of img
	i.e: 
		<img> 
		<link>
-meta tags allow otudated devices to read our websites well. Use MDN to understand them 



Eliot's fronted example: 

		<html>
			<head>
				<title> Introduction to Frontend</title>
			</head>
			<body>
				<nav>
					<button>Home</button>
					<button>About Eliot</button>
				</nav>
			
				<h1>Eliots HTML Tutorial Site</h1>
				<br>
				<main>
					<section>
						<h2>Introudction to Frontend</h2>
						<p id="html_element_p">
							Today we are focused on the parent-child relationship of HTML elements, meaning the semantic in regards to elements, and of course, on HTML itself and some of its useful tags.
						</p>
					</section>
					<section>
						<h2>Javascript Magic</h2>
						<button>Click Me!</button>
					</section>
				</main>
			</body>
		</html>


  
  
  
  todo 	12 OCT 

*Started with Career services 
  
*Goes over List 
	-ol - ordered list have numbers 
	-ul - are bullet points 
		-li are the bullet points 


* tables
	<table>
		<tr>
			<th>First Name</th>
			<th>Last Name</th>
			<th>Email</th>
		</tr>
		<tr>
			<td>John</td>
			<td>doe</td>
			<td>jdoe@gmail.com</td>
		</tr>
	</table>




todo                         16 OCT : JAVASCRIPT 

eloquentJavascript.net 
https://javascript.info/


?What is global in JS 


console.log() : Is how you enact Javascript in the Web. 
Make sure to run code within the browser while learning. 

Methods to store things: 


? statements: 


?	*Variable decleration 
		var variableOne (don't use) 

		*let variableTwo = 'This is the let variable.';
			here I am telling the cpu to store data, allowing me to reference the data later on. 
			This variable can change, by resetting what the var is equal to. 

			!Use var when you first start coding, since I won't know when said variable will change if at all.  

		*const variable Three = 'This is the const variable 
			You cannot reassign a const varibale, it remains consistent 



? Data Types: 
			 
		 
* Boolean : True / false values  

  
*Strings: 
	Are text values / words 
	You can use single or double quotes here 
	
	Some Operations are allowed on here 
		concatenation: Adding two strings together 
		Coersion: avoid at all cost; essentially is adding two different data types 
			i.e: console.log()


*Number: Number values  
	Provide us the operation function operation: Things we can do to data types based on what they are 
		-Addition, subtraction, exponentiation, division, logs, etc. 

 
* Null: meaning the absense of value "nothing"
	You have to assign null. 
 
* Undefined: refers to a value that has not been assigned yet 
 
* Bigint: Extra large box that accomodates more numbers than the number data type. 
 

 *

*Typeof: 

* Symbol: Unique identifier that re-organizes similar data by differentiating the data by  " serial number" 
 

 ?Operators: 



	*Logical operators: are used to determine if something true or false  


		&&: Checks if both conditions are true 
		||: Checks if one condition is true 
		! : Returns a false if the result is true 

		
			*&&: checks for both conditions  
			*II checks for at least one condition to be true  
			*! Returns a false if the result is true 

				Cool thing here you can !! to find a variable's truth value 
					*Six Falsy Values: Always return that they are false if asked
						0
						''
						null
						undefined 
						NaN
						false


Camel Casing: 
	const isaiasIsTheBestTeacher = true; 








	Todo 						18 OCT
	 


*	 Pair programming: is a two person activity 

		

		The Coder: 
	 	-THis person writes the code and depends on the navigator to catch errors 

		Navigator:
			-Observes the coder and calls out mistakes / gives suggestions and feedback 
			-screenshared onto the project and watching, kinda like QA 
			-The more seasoned person is typically the Nav 


			Ruber Duck Programming: 
				-When you don't have a thought partner you voice thoughts to a rubber duck to review your decision process 


		Mob Programming: 
			-4 to 6 people work together to complete task 
			-Not used often 

		Project Planning
			-When one plans the project ([pseudocode]), and thinks thoroughly before starting 
			-Improves team communcation 
			-Easy to track goals / outcomes 


				Methodologies: 

				*Waterfall: 
					Each phase passes down onto the next. 
						pros: Clear structure, clear requirements, easy to measure progress 
						cons: slow start .... you can;t make changes during development. 

						Requirements -> Design -> Implementation -> Verification -> Maintenance 


				*Agile: Someone approaches your team with an idea and you complete the smallest chunk of it. 
					The reason for completing the product in smaller bits is because tech / how valuable projects are, changes through time.
					

				*Kanban 
					There is a backlog of things to get done. Compares to Agile scrum , but is looser in the sense that there are no ceremonies, cycles etc. 


		Sprints 
			Sprints are time-boxed periods of one week to one month where a product owner, scrum master, and scrum team work to complete a specific product addition. 

				Backing: Future task  
				Inprogress: what is being worked on 
				Done: Completed task 

		Task: 
		-Finish workshop 
		-Competency check 
		-number 9 assignemnt 

		Canvas link: https://fullstack.instructure.com/courses/669
		Zoom link: https://fullstackacademy.zoom.us/j/5585775306?pwd=R3JVd1RkTFd6anI0VGZpUFo4cWkwZz09 




Todo 			19 OCT 



Michelle: 
	-Download Notion app for keeping track of meetings, comments, improves, etc 


	-How to do homework uploads on GitHUB 

		1. Create a repo on Github 
		2. Clone repo onto VSCode 
		3.Create index.html file 
		4. Create a about, contact, index, and style file -> upload it to Github 
			
				i.e: 

				<html>


todo 										23 OCT: CSS GRID 

! Assignment DUE : Make a personal Journal on GIT HUB 
! thing to research 
https://css-tricks.com/snippets/css/a-guide-to-flexbox/
https://css-tricks.com/snippets/css/complete-guide-grid/
https://cssgridgarden.com/
https://flexboxfroggy.com/


?					         CSS Grid vs Flexbox vs Boostrap 

--------------------------------------------------------------------------------------------------


*Flexbox: 

	? When using flex: Tell the 
		margin: 0; 
		height: wrap; 

	good at one demensional (either a columns or row, you can't change direction  ). 
			You can change the direction of the content 
			
	It's good to use a combo Flexbox + CSS grid when creating a layout. 

		You can give different boxes a perentage of the row/column to take up 
			
			box1: 30%; 

			or 

			.sidebar-1, .article, .sidebar-2 { 
				flexL calc(100% / 3 -10px);
				background-color: grey; 
				margin-right: 10px; 
				mnargin-bottom: 30px;

			}

! Refreshed on an old trick make sure to understand it! 



--------------------------------------------------------------------------------------------------




*CSS Grids: 

	two demensional (columns and rows , like image galleries and portfolio projects) 
				Is a newer feature compated to flexbox, so features have to be implemented manually for other browsers .. 
			


	Honestly sounds like CSS GRids is King. 

	
	Bootsrap4: Came before Flexbox and CSS grid. So it's outdated compared to the first two methods mentioned. 

! Learned a new trick ensure to review screen shot and understand it ! 
		-Grid-Template-Rows 
		-Z index: The axis of depth 
		-media Query: The adaption of content based on the pixel (screen size) that the user has. 
		*Use this to modify whatever goes out of bounds when changing pixel sizes. 

! Assignment: 
		how to create shapes in CSS: 

		Figma / Photoshop: 
			Use these to create the circles and other shapes 
		*SVG to   
			blob creator: 
				creates shapes  
		Todo 					   CSS GRID 1



		*Steps to Creating a Grid System: 
			1. You have to wrap all elements you want to Gird in <div class="container"> ..next give it them the CSS rule of: 

			2. display of: Grid; 

			3. Use the rules below to manipulate the size of the grid's pixels and the number of colums. In method 
			
			*(a) a set pixel size of columns, and number of columsn
			
			*(b) I use percentages in order to take up more of the screen. This method still leaves space to scroll 
			
			*(c) Fr value is the golden value to use when creating grids

				(a) grid-template-columns: 300px 300px 300px;
					tells your pages how many columns and what spacing 
				(b) grid-template-columns: 25% 25% 25% 25%; 
				(c) grid-template-columns: 1fr 1fr 1f2; 
				?2 This value is relative, meaning you want three columns, where the last columns is twice the size of the first two
			
			4. Use grid gap IOT create a gap between all elements. 
				grid-gap: 20px; 


		todo					CSS Grid 2 

		Rows can be defined as well 
			*1. Grid-template-rows: 1fr 2fr; 
				Any following rows will repeaet the same rule of previous rows .
			2.   grid-template-columns: repeat(3, 1fr);
					The first # is how many times you repeat
					The second # is what fr value you want repeated
			*3.   grid-template-columns: auto;
					Auto property automatically resizes to fit the content to its placement. 



		todo 					CSS Grid 3


		*justify-items 
		is a property that controls where within it's boxan elements starts at.  

			Justify-items: stretch;
				Is the default for CSS Grid, where items are stretched along the row axis. 

			

			justify-items: start;
				This aligns contents towards the start of the row. 
			
			Justify-items: end; 
				This algins contents towards the end the row in the grid system. 

			align-items: start/end
				is the same as above but along the column axis. Here you can use 


		?Preferred methods of creating a grid layout

		The instructors preferred method is derived from the style metioned below, however it allows for the website to be more responsive when using smaller pixel levels. 
		*   grid-template-columns: repeat(3, 1fr);

		Common grid patters: 
		*	grid-template-columns: repeat(auto-fill, 300px)

		Even better pattern:
			*grid-template-columns: repeat(auto-fill, minmax(200px, 1fr)
										how small columns are     max


		todo                       CSS Grid 4



		*Selecting Indivisual Items or Zones within the grid: 
			In the example  we modify backgrounds of items by the background color: 

		*Grid Column:

			.green {
				grid-column-start: 1;
				grid-column-end: 2; ->3;
			}
			?... if you change the end value to 3... Then you command for the zone to span from columns 1->3. This feature responsively changes with width of the page. 

			shorthand version 
			.green {
				grid-column-end: 1/3; 
			}

			To make the zone spand all the way to the end: 
			.green { 
				grid-column-end: 1/-1;
			}

			If you're not too sure how many total grid you'll use:
			.green {
				grid-column-end: span 2;
			}


		*Grid Row can also be used in a similar facet:

			grid-colum-end: 1/3
			grid-row: 1/3; 

			


		Todo 						CSS	GRID 5 


		Using Justify with Grid-column-end & Grid-row
			
			grid-colum-end: 1/3
			grid-row: 1/3; 
			align-self: end; 
				*This would take space of the selected grid, while also moving the green zone to the bottom Grid space. 


		Todo						CSS Layout

		* Using all of skills I've learned up until now, create a layout for a website!
			The website must have a: Header, Cover, Project Grid, and Footer that is responsive.
			Use both Flexbox and CSS grid?  
			



		todo 							Creating a Layout 


		*New Things I Learned in this exercise: 

		? vh - or viewport hieght allows you to set a responsive height to containers. this value works in terms of percentages. 50vh means said container will take up 50% of the screen.  

		? Grid Wrapper - In the index document whenever you want to use CSS Grid create a Grid wrapper class
			<div class="zone blue grid-wapper">








todo 							OCT 30th : Introduction to REACTOS


! : Look at last lesson "Block 11" I believe 

? 	REACTO


? 	Restate
		rephrase in your own worlds what the problem is 
		*its useful to use apps to draw pictues and diagrams 
		ask clarifying questions. Don't assume values at all! 
		Get answeres to assumptions, dont assume. 


?	Examples 
		Think of examples you can come up with to test the code

? 	Approach 
		come up with at least one solution 
			identify pros and cons
		Don't code, pseudocode -> pseudocode while being vocal to hints from the interviewer
		

?	Code 
		Follow the pseudocode 


? 	Test 
		Use representative input and output examples to test that the code you created can ressolve the problem

?	Optomize 
		Basically, how can I make the code better 
			Space Complexity: Is a concept which says that 


Activity: They provide an interview prompt , we follow the reacto steps, They provide feedback 



*Leetcode : 
	Is a good platform to use to practice for interviews 



todo 				Javascript 



? if else conditional statement : 
			var age = 18;
		if(age >= 65){
		    console.log("You get your income from your pension")
		} else if (age <= 65 || age >= 18){
		    console.log("Each month you get a salary")
		} else if (age <18){
		    console.log("You get an allowance ")
		} else {
		    console.log("The value of the age is not numerical");
		}



? Else if statements: 



? Function 
	are more powerful that conditional statements because they allow us to not repeat our self, instead we run it again with a new arguement 
	*	Console.log(chekcIfICanDrinkAlcohol(birthYear:2005):;
					parameter						arguement 

			

? How to generate a random number 

function randomNumber () { 

		const randPercentage = Math.randNum = Math.random(); 

		return randNum; 

}





todo 							01OCT     Arrays 


vocabulary: 
	global 




Looping Constructs


	?1. For Loop

	• Are used to continually execute a conditional code until a certain condition is satisfied. 
	
	• (i) Counter: is the specific value that the loop I looping to get. 
		○ Start count value must be assigned 
		○ N count value: How many times the loop will run , what are the conditions for it to run 
		○ incrementor:  changes the value of I on each loop evertime it runs 
		?	 i=i+1 or i++
		○ Exit conditions: what value should things terminate @? 
		○ Loop body: contains the block of code you want to run on every loop iteration
		 
		! review how to splice an item out of the loop


	


		i.e: 
			
			(1) 
				
				
				for (let i = 0; i <=5; i++) {
				    console.log(i)
				}
				console.log('Counting completed!')


			* OR 

			function favoriteDog(name) { 
				console.log('My favorite dog is ${name}!');
				? name as console.log("My favorite dog is" + name + "!")
			}

			*	for (let i=0; i < dogs.length; i++)
					console.log(dogs{i});

				
			(2)
			
				
				for (var i =5; i>0; i--) {
				    console.log(i)
				}
				console.log('Countdown finished!')
				
			
			



	2. While Loop 

	"While the counter remains true, run this code within the brackets, when the counter condition is no longer true, output this value. 

		○ Very similar to the For loop however different due to: 
			§ Counter value (set before the loop) 
			§ While (counter > 0) is the condition 
	
			
		I.E: 
				
				
			(1)
				var i = 1; 
				while (i < 6) {
				    console.log(i);
				    i++; 
				};    
				 remember to include this semicolon here, also remember to use the variables you learned in for loops
				
				console.log('Counting completed!')
			
	
	
			(2) 
				
				
				var i = 5;
				while( i > 0) {
				    console.log(i);
				    i--;
				};
				console.log('Countdown finished!')
				
				
			(3) 
			
			
				var i = 2018; 
				while (i<2023) {
				    console.log(i);
				    i++;
				};






							
							

NESTED LOOPS


	• Are when you need a loop to run within another loop. 
		○ Can be for loops,
		○ When you need to process data sets A and B at the same time. 
		
	• The loop nested within the main loop can only run as many times as the main loop runs

			(1)  for (i = 0; i < 2; i++) {
			(2)     for (var j = 0; j < 3; j++) {
			          console.log("Hello");
			      }
			  }
			
			When (1) runs x1 times (2) runs x3 times.
			
 
Example:  
 
You are coding a two week plan from Monday – Friday  where you need to:

• Populate days by number (1-5)
• And associate the says with either week one or two




todo 		02NOV		Reviewing the functions // introducing Objects


	?Objects: grant the ability to give properties and actions to variables. 

		This happens because It allows us to store various properties and actions. 
		In most cases objects properties are stoerd in a key:value format 

		
OBJECTS {}
	


	const fruit = { 
		name: "banana"
		color: ["green", "yellow", "brown"]
		sugar: 14, 
		isAvailable: true, 
		};
			?so essentially you can store values in objects, arrays, numbers, and boolean values
		Morenotes: 
			-The key, aka: name,color,sugar etc .. dictae the ____ 
			-Values, aka: banana, [green,yellow,brown] dictate the value 

		const fruit = { 
		name: "banana"
		color: ["green", "yellow", "brown"]
		sugar: 14, 
		isAvailable: true, 
		};
	}


todo 	06NOV 		Other versions of Arrays 

const fruitArray = ['🍇','🍈','🍉']
grape: 
melon: 
]

const fruits = object.values(fruitOject); 
	turns an object to and array 


 -----------------------------CLASSNOTES-------------------------------------------
?const fruitsArray = ['🍇', '🍈', '🍉', '🍊', '🍋', '🍌'];

? const fruitsObject = {
?    grape: { emoji: '🍇', price: 3.79, color: 'purple' },
 ?   melon: { emoji: '🍈', price: 3.19, color: 'green' },
  ?  watermelon: { emoji: '🍉', price: 4.19, color: 'green and pink' },
   ? tangerine: { emoji: '🍊', price: 3.97, color: 'orange' },
    ?lemon: { emoji: '🍋', price: 3.99, color: 'yellow' },
    ?banana: { emoji: '🍌', price: 2.02, color: 'yellow' },
? };

forEach

old way of looping
for(let i = 0; i < fruitsArray.length; i++){
    console.log(fruitsArray[i]);
}

fat arrow function (callback)
?fruitsArray.forEach((fruit, index) => console.log(`${fruit}: ${index}`));


fruitsArray.forEach(function(fruit){
    console.log(fruit)
})

map
? const fruits = Object.values(fruitsObject);
? const fruitNames = Object.keys(fruitsObject);
? const fruitPrices = fruits.map((fruit) => fruit.price);
console.log(fruitPrices);

reduce
?const groceryTotal = fruitPrices.reduce((sum, currentPrice) => sum + currentPrice, 0);
console.log(groceryTotal)
rounds up a number
console.log(Math.floor(groceryTotal))

filter
const yellowFruits = fruitsArray.filter((fruit) => fruit === '🍋' || fruit === '🍌' )
? const yellowFruits = fruits.filter((fruit) => fruit.color === 'yellow').map((fruit) => fruit.emoji);
console.log(yellowFruits);

find
? const grapeFruit = fruitsArray.find((fruit) => fruit === '🍇' );
console.log(grapeFruit);

slice
? const threeFruits = fruitsArray.slice(0,3);
console.log(threeFruits);



todo 				08 NOV Classes and Context 


Essentially creating a object that can be customized and called upon with a Console.log. 
when invoked, the parameters come back in the form of an object. 




todo        09 NOV: Javascript Test 


*Testing: Is basically testing the function of the code you've  written. 
	*Test Driven Development: is a software development process that follows a simple iterative cycle 


?Types of Test 

*Unit Test: is a test that checks the functionality of an indivdual unit of code. 
	pros: very fast test and only test 1 component 
	con: not able to mimick user behavior


*Integration: Testing combining individual modules and testing them as they work together. 
	i.e: Checking the integration between Mailbox and Spam Mail -> Moving mail from mail to SPAM. 
	Here you're acting like a user and testing the validity of multiple functions / components

*End to End test:
	 Mimicking a user's behavior flow to wholistically test and app 

*Acceptance: Testing that the application meets the identified requirements 
	Alpha and Beta Releases of applications or software


*Functional: Testing user scenarios on the browser itself by controlling the browser programmatically. 




	Javascript Testing Frameworks: 
		-Libraries of code used to help test JS code 
		-Provide a set of function and methods to test code for erros and bugs 
		-Ensure code is working correctly and meets specs 
		-Allows automation of testing process -> developers can spend more times developing new features etc. 



?							How to write test! 

*	1. Read the problem 

* 	2. Identify Expectations 

* 	3. Wite Psuedocode 

*	4. Translate Pseudocode to real code



*Example: 

		Write a function multiply(x: number, y: number) that returns the product of two input numbers. 

		-I expect to have a the product of two numbers
		- function(x,y) = x * y

--------------------------------------------------------------------------------------------------------------------------
? 												Blocks 11-20: Starting Fresh 


*Block 11: 

Git Workflow: The following commands are used to push things from Git to Github and enable pair programming on a main branch of Github 
its dope  because with each commit, you can track what changes were made

	1. git innit 
	2. git clone 
	3. git status 
	4. git add 
	5. git commit 
	6. git push


 Projects Organizers 
 
 	Git Projects: is a top tier orginizational tool 

*Summary: This block I learned how to use Git for pair programming. 


*Block 12

Here I used the Github Project board, CSS Flexbox, and other cool tools(listed below) to create a Upgraded Personal Website 
		proportional units
		dynamic styling with hover effects
		A contact form with the following:
		These specific fields:
		name field
		email field
		message field
		submit button



?Block 13: Conditionals and functions 


	Boolean assist in helping us make conditionals, comparisons, and logic within Javascript. 
	Variables can be explicitly defined as true or false, however they may also resemble the following Truthy/Falsy structure below 

	*Truthy Values 
		True 
		Non-empty Strings 
		All numbers except for 0
		()empty functions 

	*Fasly values: 
		False 
		"" - Empty Strings
		0 (number zero)
		null 
		undefined 
		NaN 


	*Assignment operator: 
		Essentially equaling something to something. The assignment operator (white) typically has a name that coorelates with the value (brown) 

*Types of Operators 

	=  -> assignment operator: Assigns a value to the left operand based on teh value of the right operhand 
						Color = brown 

	== Loose Equality Operator: Check the equality of the value. Javascript will attempt too convert the value if th operand are different types. 
					1 = = "1" -> True 

	=== Strict Equality Operator: Checks for teh equality if the value and type
					1 === "1" -> False 

	.!= Loose Inequality: Checks for inequality of the value 
					1 ! = "1" -> False 


	.!== Strict Inequality Operator: Checks for the inequality of the value and type 
					1!==2 -> true 


*Control Flow: 
	Is how you tell computers to make decisions. "we are controlling the flow of a program. 


*If else statements
	
		execut a statement if a specfic conditions is truthy, 
	
		Else, another statement in the clause will be executed instead. 

				const isSunnyToday = true; 
					?^This is the expression 
				if  (isSunnyToday) {
						?This space here is called a code block 
					Console.log("lets go to the park"); 
						?^this is the execution 
				else { 
					console.log("Lets stay inside and watch a movie");
				}
				}

*Else if Statements 
	Allow us to prompt the computer to ask itself multiple questions. 
		?if a else if condition is met, subsequential part of the function are not ran afterwards 


*Logical operators: are used to determine if something true or false  
		AND (&&) operator:  Checks if both conditions are true 


		OR (||) operator: Checks if one condition is true 
		
		BANG/NOT (!) operator : Returns a false if the result is true 

	2+2=4 false 
	2+x != 4 ... true .. so returns a true statement when the result is false

*Functions 
	block of code that will execute agiven task. To use it you gotta invoke or call it. 

		function sayHello() { 
		?This is the finction invocation 
			console.log("Hello there!")
		}

	Can be written two ways 

		*Function keyword 

			function sayHello() { 
				console.log("Hello there")
			}
	

		*Arrow Syntax
			const sayHello = () => {
				console.log("Hellow there")
			}

functions can be defined to take Parameters. 
		*Parameters: locally scoped variables that act as placeholders for values in functions until function is invoked and replaced with arguments 

			function sayHello(name) { 
				console.log('Hello $[name!'])
			}

			sayhello('Cody');

*Arguments: 
	are actual values passed to a function when its called. 

*The return word	
	oftentime we need functions to output values we can use somewhere else in our code. Return helps this. 
		*Return button ends function execution

		function sayHello(name) { 
	?			return 'Helllo $[name]!;
			};
		*nothing will print after this line

			Const mmessage = sayhello('Cody')

			console.log(message)



*Block 14: Loops and Arrays 


	Arrays is a data structure that stores multiple values in a single variable. It's efficient because instead of storing each veggie or number in it's own variable, we can store all of them in one. 
		

			const vegetables = ["carrots, "cabbage", "lettuce"]; 
			const numbers = [1,2,3,4,5,6]; 


? Array Manipulation (through methods)

	

	*	Slice returns a new array made of the sliced iteams wihtout taking from the array. 
			let numbers = [1, 2, 3, 4]; 
			let slicedNumbers = mumbers.slice(1, 3); 
				*This method takes both start / stop index and the end index is exclusive(meaning its not counted within the slice.)
			console.log(slideNumbers)
				Output: 2, 3


	*	Push adds elements to the back of an array. 
			let array_number = [10,20,30,40]; 
			array_number.push(50)
				output: array_number = [10,20,30,40,50]


	*	Unshift adds one or more elements to the beginning of an array while modifying the array. 
			let nunbers = [7,8,9]
			number.unshift(100);
			console.log(numbers)
				output: numbers = [100,7,8,9]


	*	Splice is a  method that removes numbers from an orginal array and places them into a deleted elements seperate array. Splice also has the capabilities of adding numbers into an array? 
				let fruits = ['apple', 'banana', 'orange', 'grape'];

				let removedElements = fruits.splice(1, 2);
				console.log(removedElements);  // ['banana', 'orange']
				console.log(fruits);           // ['apple', 'grape']


					General syntax of a splice()
						The general syntax of splice() is:

							array.splice(start, deleteCount, item1, item2, ...);

							start: The index at which to start changing the array (either add or subtract
							deleteCount: The number of elements to remove.
							item1, item2, ...: Elements to add to the array at the start index. 




*		Pop removes the last element from an array. 
			let array_number[10,20,30]
			array_number.pop(30)
			console.log(array_number)
				output: array_numbers = [10,20]


	*	Shift : removes the first element from an array. 
			let number = [10,20,30]
			number.shift(10)
			Console.log(number)
				Output numbers = [20,30]




*LOOPS 
	Give a quick and easy way to do something repeatedly. 
		Types in include For & While Loops 

		You can use them to: 
			Traverse over a large set of data 
			Repeat an action over the items in an array 
			Do something until a certain condition is met

	

	FOR LOOP: 
		loop through a block of code number of times 

			for(initialization; conditionl; afterthought) { 
				/ statement;
			}

				initialization: executed once before the execution
				condition: defines the condition for executing the code block 
				afterthought: executed after the code block finishes 


	While 
		Loop through a block of code while a specific condition is true 

			while (condition) { 
				/code block to be executed
			}

				let num = 5; 
				while(num<10) { 
					console.log("our current number is" + num); 
					num++
				}
				console.log("end of loop")
				

? Events 
	are signals which say something has occured. When an event occurs it can trigger a function or an... 
	
*Event Handler

	document.getElementById('hoverBtn').addEventListener('mouseover', sayName); 
		//


const sayNameBTN = document.createElement('button'); 
sayNameBtn.innerText = 'Click Me'; 
sayNameBtn.addEvenetListener)'click', sayName); 
sayNameBtn.setAttribute('class', 'btn'); 
sayNameBtn.setAttribute('id', 'clickBtn');

	document.querySelector(#form).addEventListener('submit', doSomething)
		e.preventDefault()
		const firstName = document.getByElementId('firstname').value; 
		const lastName = document.getByElementId('lastname').value; 



	}); 


OFNOTE: 
	You can use JS to create a button that doesn't natrually exsist in the HTML , and make a CSS to style the button. 









? Introducing: Node & Modules 

First you write the test, then you write the code to pass the test  


*Main points 

- Testing syntax: 

	- syntax: 
		see below


	*Vocabulary 
		
		-'module' in Node.js, the module object is a special object that is available in every module file. It represents the current file or module and provides a way to define exports 

		-exports within "module.exports" is an object provided by the file or module that allows for export function from one module to another 

		-sum within "module.exports = sum;" is the value of module.exports. So my assumption is we assing the value of the function we intend to test. 



* Understanding Exports and Imports : 
	
	
	
	*Exports: You export functions in file via "module.exports.(name of function)

	*Imports: You inport function by making a const variable: 
			const LuckyNumber = require('./sum');
			You can also import multiple function by doing the following: 

	const { getTotalCost, applyDiscount, applyCoupon } = require("../index.js");


					*Require method: allows us to import code 
						*Code can be one's we wrote or it can be code we downloaded


	*Exporting Multiple functions from one module: 

	*function 1: 
		function LuckyNumber(a, b) { 
		return a + b; 
	}
	module.exports = LuckyNumber; 


	*Function 2: 
	const forSale = {
		bath: true,
		bedrooms: 4,
		kitchen: {
		amenities: ["oven", "stove", "washer"],
		area: 20,
		wallColor: "white",
		"nice.oven": true,
		},
	};

?< Method that has worked:
  *module.exports.LuckyNumber = LuckyNumber;
  *module.exports.forSale = forSale;




This syntax above allows to export multiple functions 
Allows me to export multiple functions 


? How to set up and run a test in VScode 


	*	Identify a file with a function that you'd like to test: 
		sum.js: 

			function sum(a, b) { 
    		return a + b; 
		}
		module.exports = sum; 
	* export the file to the jestJS testing file  

	*	Create a file that mirrors the file you want to test
	*	Write a test
			sum.js -> sum.test.js 

		const sum = require('./sum');
*Call the file you want to test to the test.js file 
		test('adds 1 + 2 to equal 3', () => { 
   		expect(sum(1, 2)).toBe(3);
}); 

	*	Use npm run test -> To run the test! 
	- Complete ! good stuff 


			
			

	* sdf
				npm run test
-Mock and Stub 



?									Using API's 

*Application Programming Interface: 
	Application in API - refers to software that provides a sort of function. An API can be thought of as a contract of service between two applications (server and client). The contract defines how the two communicate with one another using request or responses. 
								<-
			client -> REST API -> Database 
					<-
*CRUD Operations 
	Behind the scenes APIs manipulate data... below are four basic operations a software application should be able to perform. 

	1.			create | Read | Update |  Delete 
	2.	GET 	POST   | 	  |	PUT 	| Delete
	
		1: CRUD Operations: These are the backend operations/data manipulations that need to run. 
		2: HTTP Methods to complete the methods 

*Endpoints 
	simply put, an endpoint is one end of a communication channel. When a API interacts with another system the touch point of this communication are considered endpoints 

	GET	/ users 	-> show all users 
	Get / users/4	-> show a single user(whose ID=4 in the db)
	POST / users	-> create a bew users in the DB 
	PUT	 / users/4	-> Update user 4 in the db 
	Delete /users/4	-> Delete user 4 from the db

	*sending a request to REST API with fetch 
			asyn function getUser(id) { 
				try { 
					const response = await fetch('https://api.com/users/${id}');
					const data = await response.json(); 
			?							***
					return data; 
				}	catch (error  {
					console.error(error.message); 
				}
			}

	* await 

	ELIOTS EXAMPLE: 

		const fetchGoogle = async () => { 
			const response = await fetch(input: 'http: google.com/)
			const html = await response.body.getReader().read();

			console.log('Response Body: ', html); 
		}




	? ***: THE JSON reads the body of response & returns a promise...that results in parsed JSON data. The Purpose of using JSON is -> if server returns a JSON-formatted response, the method ensures that the data is converted from JSON string to a javascript object. if not an error may occur

*REST - Representational State Transfer: 
	Architechture style that describes how an API should work 
	Created as a guideline to manage communication on a complex network (aka the internet)

*REST API is an API that follows the REST principles. 
	Endpoints should be uniquely identify an action and a resource. 

*Fetch 
	provides an interface for requesting data from other sites

*Asynchronous Programming
	Multitasking within code. Grants the ability to start long running code, and immediately move on while it finishes the task 

*The Event loop 
	Since JS is single-threaded it can't actually multitask. Instead the event loop is responsible for executing code and coordinates when each operation is allowed to happen 

		i.e: 	
			console.log("One"); 

			setTimeout(() => 
				console.log("two"), 10); 
			
			console.log("Three")

						console.log("One");: This statement is executed first, and it prints "One" to the console.

						setTimeout(() => console.log("two"), 10);: This schedules the execution of the arrow function () => console.log("two") to be executed after a delay of 10 milliseconds. However, the rest of the code continues to execute without waiting for the timeout to complete.

						console.log("Three");: This statement is executed immediately after the setTimeout is called, and it prints "Three" to the console.

						After the initial execution, the event loop will eventually reach the scheduled console.log("two") inside the setTimeout callback after a delay of 10 milliseconds. It prints "two" to the console.

						So, the final output order is "One", "Three", "two".
								

?How to Handle Asynchronous code: 

	*Callbacks: 
		when a code is passed as an argument to another code. The other code is expected to "call back" or execute the code at a later period of time. 

			console.log("Getting Configuration")
			fs.readFile('/config.json', 'utf8', (err, data) => {
										?This is the callback
				console.log("Got configuration:", data) 
			});
		console.log("moving on...");

		
	In which order will the logs fire? 
	Answer: "getting Configuration" -> moving on... -> Got configuration "data"

									
		?ofNote: 
		an "err" is passed in callback so if an error occurs, information about it is caught within the function. If not it'll be undefined. 
				If err has information, we can expect data to be undefined. 

				i.e:
					fs.readFile('/config.json', 'utf8', (err, data) => {
						if (err) {
							console.error("Error reading configuration:", err);
						} else {
							console.log("Got configuration:", data);
						}
					});```
			


	*Promises: 
		is an object with a value and a status. It represents the eventual result of an asynchronous operation. 

		The status is either pending, fulfilled, or rejected. 
			Pending: = the value is undefined 
			Fulfilled = the value is defined
			Rejected = there was an error with the operation 

		async function: decleration denotes that the function returns a promise. 

		*Await operator 
		 Is used to wait for a promise to resolve and get its fulfillment value 
			It can only be used inside an async function. 

i.e: 	
	const caramelizeOnion = async () => { 
		const onions = await getOnions("pantry");
		const choppedOnions = await chopOnions(onions);
		if (choppedOnions) { 
			console.log("Caramelizing the onions!");
		}
	}; 

*uncertainty 
	You can't trust sources to behave as expected. There are almost an infinite number of reasons something might not work as expected

		


*try/catch statements
	try is the happy path

	catch is the bad path 

	finally is the stoic path, meaing it will always run 
			consol

1.	try { 
		tryStatements
2.	}	catch (execptionVar) { 
		catchStatments
2/3	}	finally { 
		finallyStatements
	}
		
		*First the try block is executed first. 
		*If an exeption is thrown, the code in the catch block will be executed. 


const caramelizeOnions = async () => { 
	try {
		const onions = await getOnions("pantry"); 
		const choppedOnions = await chopOnions(onions); 
		if (choppedOnions) { 
			console.log("Caramelizing the onions!");
		}	else { 
			throw new Error("kitchen is burning!"); 
		}
	}	
	
	catch (error) { 
		console.error(error.message); 
	}
};


so in summary, promise statements grant the ability to await a value , and deduce a result based on the value. If unsuccessful, an error, or undefined can populate instead. 





? SPAs: Single Page Applications 
	Single page applications send over a single document and updates the content rather than sending a new document. 


* URL hash 
	is a string that starts with a # 

* Routing refers to the concept of directing users to different application views without refreshing page. 


*Hash Routing 
	refers to showing user diffrent application view depending on the URL Hash
	we can implement Hash Routing by adding an event listener to the window's hashchange event. 

	We can then update state by parsing : window.location.hash


*Hash routing: 
	This allows us to store data in the UR: to allow us to get to where we want to go. 

	You can access different versions of the page based off the hash 



		window.addEventListener('hashchange', () => { 
			console.log(window.location.hash);
		}); 



Of note on Eliott's technique: 
	-render takes whatever is on the state and runs it. 
	-sometimes when you run hash strings.. decodeURIComponent (window.location.hash) -> makes the format normal again. 

function eliott wants us to learn: 
	-accumilation patter
	-loop over something and build a new array


Assingment Eliot is going to create: 



-Start the app with startapp
-hash changes the stae 
-render 
	single page application that we continously update
	

THis week is the last week to master Javascript


attempting to append CardImage: 

	*        playerCard.appendChild(cardImage);
	* 		 const cardImage = document.createElement('img');
       		 cardImage.textContent = player.imageUrl // Set the player image


Next Week 

	-React 
	-Express 
	-Node





todo 			Functional Programming (FP)  / Higher-Order Functions

FP: programming a way a developer can solve a problem. This way or method focuses on the application and composition of functions

				Fp is Pure or Side-effect-less 
				
					Side effects are a byproduct or result that occurs due to storage of a value in a OOP function, versus just making that function directly

				Fp also has a strict control flow meaning 
					This means that input is directly mapped to output without a value 

		i.e: 

?									FP vs. OOP 

*OOP : produces events outside of its own body and effects something( Computer memory... think of the negative effects of this when scaling)

	? OOP are good whne you have a fixed set of operation on things (think PuppyBowl)

		define squared_sum(x,y) { 
			sum = x + y 
			squared sum = sum^2
			return squared;
		}

*functional programming: Pure function, no side effects , no weird bugs to figure out, no system memory used  
	? Fixed set of things and as the code evolves you add you add new operations on those existing things. 

		define squared_sum(x,y): 
			return (x+y)^2 



* Functional Programming Basics 

	First class functions are: 
			- Assinged to a variable
			-Passed as an argument 
			-returned from another function

			*Assigning a Function to a Variable: 
					You can assign a funtion to a variable name. It will store that information in the variable name... I can later use that word with curly braces to invoke the function. 

						i.e: 
						const display = () { 
							console.log("display message");
						}; 
						display()


			* Passing a function as an arguemnt 
				A function can be passed as a parameter to another function and can be executed by it.        


			*This is the function that will be past into another ... 
				function displayMessage()    { 
					return "Hello world, "; 
				}

			*Below describes the structure of the GREETING function, which will recieve the other function... 

				function greeting(displayFunction, message) { 
					console.log(displayFunction() + message);
				}

			*
				greeting(displayMessage, "Passing a function as an arugement!"); 
					? Here "displayMessage" is being passed as the display function in the greeting function.

					Console.log result: 
						Hello world, Passing a function as an argument! 
				
					* So we can say that one function is returning another function. 
					* the greeting function is returning the displayMessage function. 


* Currying: the concept where you pass in functions once at a time 


i.e # 1
const buildSandwhich = (ingredients1) => { 
	return (ingredient2) => { 
		return (ingredient3) => { 
			return `${ingredient1}, ${ingredient2}, ${ingredient3`}; 
		}
	}
}

		const mySanwhich = buildsandwhich("Bacon")("Lettuce")("Tomato")
		console.log my sandwhich 


i.e # 2

		const multiply(x, y) => x * y; 

		const curriedMultiply = x => y => x * y; 

		console.log(multiply(2,3)); 
			= 6

		console.log(curriedMultiply(2)); 
			* y => x * y  ,, the function will be console.logged until the parameters are completed. 

		console.log(curriedmultiply(2), (3)); 
			=6 

https://www.youtube.com/watch?v=I4MebkHvj8g (more to follow on curry)



? 									Closures 

	functions that can access values outside of their own curly braces.
	closures are functions that are combined with their lexical environment (outer environment)

 
		function pureFun(a, b) { 
			return a + b; 
		}

		-When this function is called, it goes to the call stack and the memory is temporarily saved, until its popped back off the callstack. 

	let b = 3; 

	function pureFun(a, b) { 
			return a + b; 
		}

		-If this function instead references free variables from the outside environment, then something cool happens... 
			- The interpreter knows in order to complete this function it has to create a closure to store the information, so it can later access it. 

				- That closure is called a heap memory. 
				-Heap memory is long lived, and can keep memory and data indefinitely. 


 todo understand the callback function: in 	Higher Order functions 

		function higherOrder(callback)
		{
			**perform some operation
			** Call the callback function
			callback();
		}


todo understand Partial Application / why its effective


todo understand composition 


todo understand high-order function 



? 						State and Props 


		https://www.google.com/url?q=https://react.dev/learn/passing-props-to-a-component&sa=D&source=editors&ust=1702788234140254&usg=AOvVaw33f45EhCISeAcvTKN833ZH


*State: The memory of changing components which retains the data

	*State setter function 
		Allows us to update the variable and trigger REact to render the component again. 


*Steps to Using State: 

	1. Import useState from reach at the top of the file: 

	2. let variable = 0; should be replaced with 
		const [index, setIndex] = useState(0);
			? ^ array         ^ deconstructors 


*Array deconstructors
	 allows us to read values from an array, the array returned by useState always has exactly to items. 

	 		this is how they work together: 
				function handleClick() {
  				setIndex(index + 1);
			}

		i.e: 

				import { useState } from 'react';
				import { sculptureList } from './data.js';

				export default function Gallery() {
				const [index, setIndex] = useState(0);

				?function handleClick() {
					setIndex(index + 1);
				}

				let sculpture = sculptureList[index];
				?return (
					<>
					<button onClick={handleClick}>
						Next
					</button>
					<h2>
						<i>{sculpture.name} </i> 
						by {sculpture.artist}
					</h2>
					<h3>  
						({index + 1} of {sculptureList.length})
					</h3>
					<img 
						src={sculpture.url} 
						alt={sculpture.alt}
					/>
					<p>
						{sculpture.description}
					</p>
					</>
				);
				}



	



*UseState or "hook". 
	1. We can add State values to components with the 
	2. Below we may need to share this user data throughout our application. 
			a. You cannot call hooks inside conditions, loops, or nested functions. 
			

			function App () { 
				const [user, setUser] = useState ({}); 
?I want you to remember ^   .. is what the useState is telling REACT here. 
				return (
					<div>
						<p> Welcome </p>
				);
			}


	3. You can have as many state varibale as you like. 
	4. state is local to a component instance on the screen. Meaning rendering two copies , and changing one of them will not affect the next. 


*Props 
	-Props in React are inputs that you pass into components. The props enable the component to access customised data
	-Parent components can pass information to child components by giving them props. 

	-props look like HTML attributes 
		i.e: 
			1. className= "profile-image"
			2. src= "/images/profile/jpg" 
			3. alt="user profile pic" width={100} hieght="100" 


*Passing information through props 
	You can pass any value through them, such as objects, arrays, and functions. 

			function App () { 
			*	const [user, setUser] = useState ({name: "Shelly", age: 35}); 
														?props^^^^^^
				return (
					<div>
						<p> Welcome {user.name}</p>
						*<Profile user={user} size={300} imageUrl="/images/profile.jpg"/>
					</div>
				);
			}			 

	In our profile component those props we passed are now available


*Accessing props 
	To access individual props we have to reach into the props object: 
		props.user / props/size / props.ImageUrl 



		*Object deconstruction: 
			A tool use to help us save time 

				function Profile ((user, size, imageUrl)) { 
					return ( 
						<div>
							<p> 
								Hellow my name is {uiser.name} and I am {user.age} years old.
							</p>
							<img src={imageUrl} alt="profile image" height={size} width={size} />
					);
				}




? 					React CDMs

* Creating a React application with Vite
	npm create vite@latest
		-proceed to follow instructions 

*Creating a repository in CDM and adding it to Github
	1. create the react app with the instruction above
	2. Add and commit files: 
		git add 
		git commit -m 'initial commit' 
	3. push exsisting repo
		git remote add origin ***link to repo***
		git branch -M main
		git push -u origin main


*Opening the REACT Live server	
	Look at the package.json app and see what scripts you have  
		- If you have vite, you can do npm run dev to get the link of the live workspace

	








? 					Fetching Data and useEffect 



TA / Instructor conversations about react: 

	-Vite is better than CRA(create react app)
	-Use state is a hook used to save information and to listen for changes within the page. 




*Vocabulary & Understandings I should be tracking: 

	1. What are props: 
		Props are attributes that can store memory or "state", and enable us to pass down certain states to child elements 

	2. What data type is PROPS?
	 	Doesn't have a data type, can be object, array, number, etc. 


	3. We pass props through deconstruction syntax. 


	4. Dependencies are all external values references within the useEffect

	5. reactive or state values, ,must be included within the UseState as dependencies 	

*Effects 
	Are used to step out of the REact code into some external system (API network)

	They enable us to run code after rendering so apps are in sync with the external system.


	"we have experienced event handlers perform "side effects" baed on user action.. 
	"sometimes we need to specify effects caused by rendering, instead. 







* Fetching Data and useEffect 

	is used to sync with external systems 

	useEffect: tells React that your component needs to do something after render. React will remember the function you passed and call it later after performing the DOM updates.



*syntax: 

useEffect (() => { 
	async function fetchData() { 
			try { 
				const response = await fetch("SomeAPIURL");
				const result = await response.json();
			}	catch (error) { 
				console.error(error);
			}
		}
		fetchData()
			? here is where you define the useEffect Function 
	}	[]);



	*optimization and resolving race conditions 
		race conditions are when network response arrive in a diffrent order than when initially sent. 

	to mitigate race conditions





Career Services: Resumes

-Resume has to have quantifiable metrics not just a job description 





? 						Tokens  & Forms 

*Vocabulary: 

Authorization checks if you have the right status to do certain activities. 


*Goal:
- How to recieve token 
- and what to do with it 

*Example Used: 
	Sign up makes an API request to get token 
	Login is a GET request that utilizes the token... In the class example she returned the username and password 








?MaterialUI (MUI)

https://www.youtube.com/watch?v=FB-sKY63AWo


? Creating a quick dashboard 


* Start by running the following command: 

npx create-react-app my-dashboard
cd my-dashboard

* For advanced navigation research and install: 
	npm install react-router-dom axios 

		

npm start
    Starts the development server.


  npm run build
    Bundles the app into static files for production.

  npm test
    Starts the test runner.

  npm run eject
    Removes this tool and copies build dependencies, configuration files
    and scripts into the app directory. If you do this, you can’t go back!

We suggest that you begin by typing:





Happy hacking!

------ 
Check that the dashboard was installed correctly: 

 npm audit fix --force

Run `npm audit` for details.


? Guided Practice 


*Setting up: 

Downlaod the MUI: 
	npm install @mui/material @emotion/react @emotion/styled

	


is the the REACT UI component library that implements Google Material Design 

*Othr React Component Libraries include: 
	-React Bootstrap 
	-Ant Design 
	-Tailwind UI 
	_Tailwind UI Kit 

* 	SassyCSS (SCSS)
	is CSS with added functionality. In SCSS you can define


		Demonstration: creatinng a login form with Material UI: https://mui.com/material-ui/getting-started/



?	 React Forms 
	

		return ( 
			
			<>
				<h2>Sign Up</h2>
				<form action="">
					<label> 
						Username: <input value={username} Onchange ={(e) => setUsername(e.target.value)} />  
					</label>
					<label> 
						Password: <input /> 
					</label>
					<button>Submit</button>
				</form>
			</>
		)

		}

*Callback functions 



*ingraining the Onchange function to memory  

		Onchange ={(e) => setUsername(e.target.value)} /> 
			The "e" or eventHandler has information about the event i.e: 
				where it occured, what type of event it is... essentially makes the event not repeat. 

		target: the target property refers to the DOM element that triggered the event. 



? 	Deploying REACT Apps to Netlify: 
			

		Run the following commands within the directory of the vite-project 

		*0 npm start
    		Starts the development server. de

		*1.   npm install 
				This allows for the build or dist folder to be created. This folder is where all files are held

		*1.5 npm run build 
				This creates the dist folder where the project will be 

		*2.   cd into the build or dist folder 

		*3.   zip -r build.zip .  
				'The -r flag stands for recursive, which includes all files and subdirectories' .. 
				essentially, run this code and a zip file will be created with all compressed data. 

		*3.5 Open <dist path> 
		       *    open .  -> if in dist folder already  
			opens the file folder in finder from terminal 

		*4. Open netlify.app and navigate to the drop file to deploy new app option. 

		*5. Drop file and wallah! Your react app is now deployed. 




? Michele's review: 

*Workflow 
	make elements, then make dummy data, make logic (functions, then use useState or UseEffect, following the css 


*integrating Data
	Data has to be able to go into the shell of as a prop ({ like this })


? React Reddux App 

On new folders you might also need to create an .eslintrc configuration file. You can do this by either using the VS Code command Create ESLint configuration or by running the eslint command in a terminal with
	*npx eslint --init.

	*Undestanding why Redux is affective: 
		Redux is framework that manages the UI and state. It syncronizes the two and ensures that the UI is always showing the most modern data from on wep apps; 

		Web apps are called web apps becuase they are rendered on the client side. In opposed to being rendered on the server(In this case JQuery will pass over the server side application to the website, thus creating a webpage. )
		
		Redux is affective because it allows developers to solely focus on building code

	*opening a new Reddux application: 

		1. Create a new reddux application: 
		npx degit reduxjs/redux-templates/packages/vite-template-redux my-app

		1b. 
		If you are in a exsisting project, run the following command to start the app:
		*npm install react-redux


		* npm install @reduxjs/toolkit
		Allows you to intall redux toolkit 

*How to set up the project 
	├── src
│   ├── App.jsx
│   ├── App.css
│   ├── index.jsx (or main.jsx)
│   ├── index.css
│   ├── store.js (or store folder)
│   ├── API
│   │   └── index.js
│   ├── components
│   │   ├── AllPlayers.jsx
│   │   ├── NavBar.jsx (Optional)
│   │   ├── NewPlayerForm.jsx
│   │   └── SinglePlayer.jsx
│   └── [other folders and files TO INCLUDE CSS FILES

more information on setting up a Redux app:  https://fullstack.instructure.com/courses/669/assignments/36204?module_item_id=254571#:~:text=out%20this%20resource-,here,Links%20to%20an%20external%20site.,-.

*Workflow for creating a Redux-React App
	1. App.jsx 
	2. main.jsx
	3. store.js -> configureStore 
	4. ``




todo: Redux Terminology and their explinations: 

*compression middleware
reduces the size of reponses and data transferred over the network  conserving bandwidth 

*What is Middleware?
Before diving into Morgan specifically, it's essential to understand what middleware is in the context of Node.js and Express.js. Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. These functions can execute any code, make changes to the request and response objects, end the request-response cycle, and call the next middleware function. Middleware is used for logging, authentication, body parsing, and much more.

*What Morgan Does
Morgan is middleware that logs requests made to your web application. It's very helpful for debugging and monitoring purposes because it lets you see what requests are being made, when they're made, and details about these requests (like the HTTP method, URL, response status, and response time).


*configureStore() 
	wraps createStore to provide simplified configuration options and good defaults. It can automatically combine my slide reducers ,
	
	configureStore returns a Redux store that is ready to use. This store has the standard Redux store API, including dispatch, getState, subscribe, and replaceReducer methods.


	"Store.js"
		import { configureStore } from '@reduxjs/toolkit';

		const store = configureStore({
			reducer: {
				sliceName1: sliceReducer1,
				sliceName2: sliceReducer2,
				?more slice reducers as needed
			},
			middleware: (getDefaultMiddleware) => getDefaultMiddleware().concat(myMiddleware),
					?An array of middleware functions to be used in the Redux store. Middleware is used for logging, crash reporting, performing asynchronous tasks, etc.

			devTools: process.env.NODE_ENV !== 'production',
			preloadedState,
					?A boolean that indicates whether Redux DevTools should be enabled. It's typically enabled in development environments and disabled in production.
					?By default, configureStore automatically enables Redux DevTools if they are available.
			enhancers: [myEnhancer],
					?An array of store enhancers. Store enhancers are higher-order functions that add additional capabilities to the store, such as the Redux DevTools extension.
		});



			*...In this example, configureStore is used to create a Redux store with a single reducer, counterReducer. The store is then exported for use throughout the application. configureStore takes care of combining the reducers, setting up middleware, and enabling Redux DevTools, making it easier to set up and maintain the Redux store.




=================



*createSlice 
	The createSlice function is a part of Redux Toolkit, a library that simplifies Redux development. It allows you to define a piece of your application's state, known as a "slice," along with the reducers and actions needed to update that state. Here's the general syntax and explanation:


	transactionsSlice.js:

			import { createSlice } from '@reduxjs/toolkit';

			const slice = createSlice({
				name: 'sliceName',
				?A string that identifies the slice. This is used in action type strings and should be unique across your application.
				initialState,
				?The initial state value of the slice. This can be a number, string, object, array, etc., depending on the data structure of your slice.
				reducers: {
					reducerName1: (state, action) => {
						logic to update state
					},
					reducerName2: (state, action) => {
						logic to update state
					},
						?more reducers as needed
						?An object containing reducer functions. Each key in this object represents an action type, and the corresponding function is the reducer that handles that action
				},
				extraReducers: {
					optional: handle actions defined outside this slice
				}
			});

		export const { increment, decrement } = counterSlice.actions;
							?this is how you export the reducers

		export default counterSlice.reducer;
			?here you export the actual function and reducers itself 



---------------------------------



*createReducer()
	createReducer is a function provided by Redux Toolkit that simplifies the creation of reducers in Redux. It allows you to define the logic for updating the state in response to actions in a more readable and less error-prone way, especially when dealing with immutable update logic. 

	Redux Toolkit's createReducer uses Immer under the hood, which allows you to write reducers as if you were mutating the state directly. Immer takes care of applying the changes immutably.

		import { createReducer } from '@reduxjs/toolkit';

const initialState = /* your initial state here */;

const myReducer = createReducer(initialState, (builder) => {
    builder
		?A "builder" callback function that defines how the state is updated in response to actions. The builder provides methods like addCase to handle specific actions.
        .addCase(actionType1, (state, action) => {
            ?Inside the builder callback, you use addCase to associate specific action types with reducer functions. Each reducer function takes the current state and an action as arguments and updates the state accordingly.

			 ?The action types passed to addCase can be string constants or action creators generated by createAction or createSlice.
        })
        .addCase(actionType2, (state, action) => {
            ?logic to handle actionType2
        })
        	?add more cases as needed
});


		createReducer example: 

			import { createReducer } from '@reduxjs/toolkit';
			import { increment, decrement } from './counterActions';

			const initialState = 0;

			const counterReducer = createReducer(initialState, (builder) => {
				builder
					.addCase(increment, (state) => state + 1)
					.addCase(decrement, (state) => state - 1);
			});

			export default counterReducer;


	*Switch statements
		*switch expression 
		evaluates an expression once and compares the result with values in each case statement. 

		*case clauses 
		different conidtions that are check against the value of the expression. if the values matches a case, the code within that case is executed 

		*Break Statement 
		After executing the code for a matching case, the break statement stops the switch statement from falling through to the next casees. if break is ommited the switch statement will continue executing the following cases regardless of their match until it finds a break of reaches the end of the swithc block. 

		*Default case: 
		This is an optional case that runs if none of the case values made the switch expression. Think of the else statement in a if else chain 

			example: 

				let fruit = 'apple'; 

				switch(friuit) { 
					case 'apple': 
						console.log('Apple is $0.99 per pound.'); 
						break;
					case 'banana': 
						console.lxog('Banana is $0.59 per pound'); 
						break;
					case 'cherry': 
						break; 
						console.log(Cherryies are $2.99 per pound'); 
					default
						console.log('Sorry, we are aout of ' + fruit + '.'); 
				}
					Note: This will log "Apples is $0.99


*Other configureStore related knowledge:
*createAction() 
	generates an action creator function for the given action type string 

*createSlice()
	accepts an object of reducer functions,
	a slice name 
	and an initial state value
		then automaticall generates a slice reducer with corresponding action creators and action types. 

*combineSlices() 
	combines multiple slices into a single reducer, and allows "lazy loading" of slices after inialisation 

*createAsyncThunk: 
	accepts an action type of string and function that returns a promise, and generates a thunk that dispathces pending/fulfilled.rejected action types based in that promise... This is used with async functions 

*createEntityAdapter 
	generates a set of resusable reducers and selectors to amage normalized data in the store 

*createSelectors utility from Reselect library re-ported for each of use. 


*RTK Query: 
	is provided as an optional addon within the redexjs/toolkit. It purpose-built to solve the use of case data fetching and caching. supply a compact, but powerful toolset to define a API interface layer for my app. It is intended to simplify common casees for loading data in a web application, eliminating the need to haandwrite 


	*Useful RTK code: 

		*data.data?.<array you are attempting to get information from>
			data.data?.players: This part of the expression attempts to access players on data.data. 
			The optional chaining operator ?: is used to safely access properties on an object that might be undefined or null. If data.data is null or undefined, the expression will short-circuit and return undefined without throwing an error.

			|| []: The logical OR operator is then used to provide a fallback value. If the left-hand side of the || is a falsy value (such as undefined, null, 0, false, NaN, or an empty string "")... if data.data does not exist, or if data.data.players is undefined or null, then an empty array [] will be returned.

		* const handleChange = (e) => {setFormData({ ...formData, [e.target.name]: e.target.value }); };

			[e.target.name]: e.target.value is a computed property name syntax that allows you to set a property on an object using a variable. 
			
			e.target refers to the DOM element that triggered the event (the input field), e.target.name is the name attribute of the input field, and e.target.value is the current value of the input field.

The object { ...formData, [e.target.name]: e.target.value } combines the existing form data with the new value from the input field that triggered the event, updating the property that corresponds to the name attribute of the input field.
? Understanding Redux even more: 

*The redux store: 
A store is a JavaScript object with a few special functions and abilities that make it different than a plain global object:

The store is the center of the Redux toolkit

You must never directly modify or change the state that is kept inside the Redux store
Instead, the only way to cause an update to the state is to create a plain action object that describes "something that happened in the application", and then dispatch the action to the store to tell it what happened.



? Routes! 
	Routes allow us to send the user to different pages within a SPA (single page application). 

	*Steps to creating a Route: 



*Vocab: 



Questions: 
	How does Redux work with useState: 
		*Ryan's advise: RTK: which is a data fetching and caching tool. 
		*Load data in with a fetch request




?Continuous Integration: 


	automating the Quality Assurance of code. 

	CI Involves automating the process of: 
		
		1. Building the code
		2. Testing the code 
		3. The CI runs automated test to check for errors 
		4. The software reports the results back to the developer 


	Yamal 

*GitHub CI 

		In Githhub, unders Repo, under Actions, you can get access to all your CI's. 


	*Github Actions 
		is used to automate sotware development workflows 
		developers can create custom workflows triggered by events such as commit, pull request, issues, and more. 


	*workflows 
		refers to a customizable automatic procedure designed to execute multiple task or jobs. 

	 
	screen record link: https://www.loom.com/share/9cd26987178d4ba49b99811560a381e5


git rebase main 




? BACKEND !!! >:) 


*Express.js
		 is a web application framework that helps devs quickly and easily create web applications and APIs 

			You can use express.js in a Node.js runtime to create robust, feature-rich web applications and APIs 



*Creating an API with express 


		*npm init -y
			initializes a new node.js project and creates a default 'package.json file. The -y is for yes - this tells npm to use defauly values for all questions in its initialization process 
		*npm i express 
			you can verify that it has been installed because you should be able to see it in package.json 
			
		*create a js file  
			typically if it's a server it'll be server.js .. you can also name it app.js 
		
		*npm install --save-dev nodemon 
			nodemon  is a package that allows for auto fresh of the page after changes have been made 
						
		 *"start": "<name of you js file>"
			within scripts place the code above so that nodemon is integrated. 

	
		*paste: http://localhost:<port#> into the insomnia project to see the server 


	
				

				



* USING INSOMNIA: 
	Insomnia is a open source application that assist with building API design and request 

		
		* http://localhost:PORT#/ 
			paste this into the and press command+enter to see you server inside in the insomnia app

		*Go into "Manage Environments" access the JSON file and add 
		
							{
				"host": "http://localhost:8080"
			}


			It is common pratice to define the base URL of the API as an environment variable, so I can easily change what follows rather than having to reset the entire URL when moving through different routes. 
				* you can then just do ctrl+space to access the e.v saving so much time! 

		*My first app: 

			server.js: 
				const express = require('express');
				const app = express();
				const PORT = 8080;
				const students = ['isaias', 'Neo', 'Future', 'Hendrix', 'Morpheous', 'coolio'];

				app.get('/hello', (req, res) => {
					res.send('Hello World!');
				});

				app.get('/hello/names', (req, res) => {
					res.status(200).send(students);
				});

				app.post('/hello/names/:studentName', (req, res) => { 
				const studentName = req.params.studentName;
				students.push(studentName); 
				res.status(200).send('Student: ' + req.params.studentName + ' has been added to students!'); 
}); 

				app.listen(PORT, () => {
					console.log(`Server is running on port ${PORT}`);
				});




* Revisiting CRUD: 
	
	Get: fetch information ... usually a 200 code 
	
	POST: save details to data base ... usually a 201 
	
	PUT: update existing information.. this replaces the entire exsting data .. 200 
	
	PATCH: update existing information..this does not replace the entire exsisting data .. 200  

		If you have a user resource with fields name, email, and age, and you want to update just the email:

			With PUT, you would send the entire user object with the updated email and the original name and age to ensure they remain unchanged.

			With PATCH, you would send just the email field with its new value. The server would update only the email field and leave name and age untouched.


	DELETE: Deleting information from a server .. usually a 204 

*Client / Pool 
	Is what allows me to interface between express app and postgres application. 
	Essentially the messenger between Tables rows and endpoints 
		Pool: is for scalability, as it has multiple clients interfacing with the table -> endpoints

*HTTP Status Codes: 



		*GET (Read):

			200 OK: Successful request and response.
			404 Not Found: The requested resource was not found.
			304 Not Modified: The client can use cached data.
			
		*POST (Create):

			201 Created: The request was successful, and a new resource was created.
			400 Bad Request: The server cannot process the request due to a client error (e.g., malformed request syntax).
			409 Conflict: The request could not be completed due to a conflict with the current state of the resource (e.g., duplicate resource).
			
		*PATCH (Partial Update/Modify):

			200 OK: The request was successful, and the resource was updated.
			204 No Content: The request was successful, but there is no content to send for the response.
			400 Bad Request: The server cannot process the request due to a client error (e.g., malformed request syntax).
			404 Not Found: The requested resource was not found.
			
		*DELETE (Delete):

			200 OK: The resource was deleted successfully.
			202 Accepted: The request has been accepted for processing, but the processing has not been completed.
			204 No Content: The resource was successfully deleted, and there is no content to send for the response.
			404 Not Found: The resource cannot be deleted because it was not found.
			
		*PUT (Update/Replace):

			200 OK: The request was successful, and the resource was updated.
			201 Created: The request was successful, and a new resource was created (if the resource did not exist previously).
			204 No Content: The request was successful, but there is no content to send for the response.
			400 Bad Request: The server cannot process the request due to a client error (e.g., malformed request syntax).
			404 Not Found: The resource cannot be updated because it was not found.
			These status codes provide a standard way for servers to inform clients about the result of their requests, making it easier for clients to understand the outcome and take `appropriate action.

	*Node.js 
		is a javascript environment that enables us to create server-sider applications with ease


? API ROUTES: 
	
	*Today's Goals: 

	*Tools used to test APIs
		
		?Postman / Insomnia (app)
			is a tool that can be used to make HTTP request to an API. It can be used to test the functionality of an API as well. 
		?Curl (CMD)
			a command-line tool that can be used to make HTTP request to an API. It can be used to test the endpoints of an API, as well as used to debug the API request and responses 
		?Fetch(Javascript)
			The web API and fetch() method can be used to make HTTP request for testing and bebugging. but mostly development.


	*API
		is the midpoint between a server and database. Rememeber for the API we use express. 

	*Server 


	*RESTFUL 
		Representational State Transfer 
			A type of web service that uses HTTP request to complete CRUD operations 
	
	*CRUD: 
		-the way we communicate with APIs and servers (GET,POST,PUT,PATCH,DELETE)
		-Remember that each CRUD operation requires it's own route to the server to request and return information. 
			GET -> /product 
			GET -> /product/{id}
			POST -> /product/{id}
			GET -> /product
			PATCH -> /product/{id}
			DELETE -> /product/{id}
		-Goes over the diff between put and patch
		
	*Distinguishing PUT and PATCH: 

			*PUT: 
				You need to submit a request with body content 
				-You DON'T get a successful response with Body content
				-is not safe? 
				-Is idempotent
					Meaning the result of a request IS sucessful with multiple submissions

			*Patch: 
				-You need to submit a request with body content 
				-You Do get a successful response with Body content
				-is not safe ? - not sure what the PPT meant by this 
				-Is not idempotent
					The result of a request may not be sucessful with multiple request submissions. 



	*Testing the API
		Primarily you can use Postman and Insomnia to test your API 
		Secondarily You can use curl from the CDM ->  localhost:8080/theResofyour URL .. 

	*Understanding Try Catchh with servers 

		? express.js try / catch blocks are used to handle errors in Express,js apps 

			*Try - obviously containing the code that may throw an error 

			*catch - the block that recieves the error. and will execute code describing it if and error is thrown. 

				*These features allow apps to handle errors and mitigate app crashes


			?Eliot encourages to start a server like such: 
				Here he makes an async await that cathes errors after connecting to the DB

						const startSErver = async () => { 
							try { 
								await startDB(); 
								app.listen (PORT, hostname: () => { 
									console.log(`Server listening on PORT:${PORT}`);
								});
							}	catch (e) { 
								console.log('Failed to start database or server. ' , e )
							}
						}; 



		PagerDuty: 	If you do not try catch async await calls on the server you can't refresh it .. 
		 it will break the server and you have to fix it, on your computer. 
 
	*middleware 
		These functions are executed before a request is sent to the server. 

		it's job is to look at request, LOGS the request/checks things, then continues to pass the request to where it needs to go to. 

		*next()
			within the express app passes the client request to the following route handler


			*Common uses: 
				-handle errors 
				-logs request 
				-authorization 
				-JSON parsing 
				-Static files 
				-App routing 
	
	!DATABASES !!!! 
		

		are locations that collect data in a organized and structured way. 
		A standard modern features include : 
			-structured 
			secure 
			efficient 


		Database can get deleted once servers go down. This is why we cannot store information on it without backing it up. 

			Databases as a result write data onto hardrives so it can be referenced. 
			FUNFACT: For this class we will be writing to your own hardriver


	There are two types of databases: 

		*Relational Databases (SQL Database)
			-stores data in rows and tables 	
			-secure
			-Connects data from different tables using "keys" 

				*Common Relational DBs: 
					-SQL 
						PostgreSQL 
						SQL  Server - Microsoft 
						Maria DB

		*Non relational Databases 
			
			-Everything else. Stores data in a way that works best for the date being stored. 
			-Does not use keys, is 'tabular'. 
			-we write what is suppose to go into the column, then we write the columns 

		Types of NR Databases: 

				*Common non-relational databases:
					-DynamoDB - key value pairs 
					-Cassandra - Column family 
					-Redis - Graphs 
					-Document model (MongoDB) - Document model 
					-firebase -  a cloud DB allowing stores data between users in real time 
					-CouchDB  - open sources DB document that collects and stores data in JSCON based doc    formats 

			
		*SQL 
			a programming language that is used to comm with and manipulate database. 

			data is stored in one of more tables(relations) of columns and rows. making it easy to see and understand how differnt data structures relate to each other 

			created by IBM in 1970s 



	*PostgreSQL
		also known as Postgres is a free O.S relational DB management system emphasizing extensbility and SQL compliance 

			they offer pgAdmin - a DB management tool with graphical user interfaces 

	*PERN Stack 
		?A Popular stack for full stack web development. 
			PostgreSQL
			Express.js 
			React.js 
			Node.js 

					NOTE: we are using PERN , but .... PostgreSQL can be used with a variety of other API layers such as PHP, Java, Python, etc... as well as front end solutions like Vanilla JS, Angular, and Vue.js(component based and declerative based programming model that nbuilds on top of HTML and CSS)  etc 

	?FLOW OF THE PERN STACK: 

		Client hits up the (UI/Code/Server URL)-> 
			Browser hits the (Actions/Request) -> 
				Server hits the (SQL queries) -> 
					Database 



?Postgres Commands: 

* \q 
	exits  psql 

find out what psql is running: 
	*ps aux | grep postgres

connect to psql: 
	*psql -U jsjulio -d postgres

find the data directory where psql is running: 
	*SHOW data_directory;

	result was: 
		/opt/homebrew/var/postgresql@15


my username:
	*user jsjulio / isaiasjulio. 

drop databse 
drop database "classroom_manager"; 


to log the messges of the server: 	
	*	pg_ctl -D /Users/isaiasjulio/Desktop/Code/psql_data -l logfile start

				ofnote: This command will start the PostgreSQL server with the data directory you specified during initialization. The -l logfile option specifies a file to log server messages, which is helpful for troubleshooting and monitoring the server's operation.
	
	To initialize a new PostgreSQL database cluster, you use the initdb command: 
		*initdb -D /path/to/your/datadir

	*After initializing your database cluster, you can start the PostgreSQL server with the following command
		
		 pg_ctl -D /Users/isaiasjulio/Desktop/Code/psql_data -l logfile start
				
	*To stop the running PostgreSQL server, use:
		pg_ctl stop -D /path/to/your/datadir -m fast

				OfNote: the-m option specifies the shutdown mode...Fast immediately terminates the connections but waits for the transactions to finish. 

	*Restarting the server can be necessary for applying configuration changes or updates. Use:
		pg_ctl restart -D /path/to/your/datadir -m fast


	*Reload server configuration: This command reloads the configuration settings without interrupting the server's operation.
		pg_ctl reload -D /path/to/your/datadir


	*To check whether the PostgreSQL server is running, use:
			pg_ctl status -D /path/to/your/datadir


	*If you're using streaming replication and have a standby server, you can promote it to be the new primary server with:
		pg_ctl promote -D /path/to/your/datadir


	*logrotate: Rotate the Server Log Files: To rotate the log files, which is useful for managing log file sizes and for log retention policies, use:
		pg_ctl logrotate -D /path/to/your/datadir


	* kill: Send a Signal to a Process If you need to send a specific signal to a PostgreSQL process (for example, to terminate a stuck backend), use:
		pg_ctl kill QUIT process_id
				Here, QUIT is the signal you're sending, and process_id is the PID of the PostgreSQL process you want to signal.





? Postgres Workflow 

	*psql -U jsjulio -d postgres
		Log into PostgresSQL as a super user
		Ensure PostgreSQL is running ( \L)
		Create a database (see below)

	* CREATE DATABASE <database name>  || createdb <data base name >
		in the case this glitches, make sure to quit and re=enter the application. 
	
	*Download repository 

	*install npm i 
		to install the dependencies 

	*npm install pg 
		download the pg modules into my project' node_modeules directory 

	* create seed / npm run seed 
		seed the db with info 
	
	* "scripts": { "seed": "node ./db/seed.js }, 
		- seed the db with inital data via the seed script 
		- ./db/seed.js is the relative path to a file named seed.js. 
		- This file contains js data
		- The file contains data JS code that connects to a psql db ann inserts data into it

	*npm start to being the server 

	* Got to global inde.js files and id the port #

	*navitgate to insomnia set up the env and your're good!  

? 	Cached and Library  08FEB2024

		*Cached: Storing information for future request 
		*Dictionary 
			*interesting stuff: flightlines give you a price based off your IP address 
		

? block 32 GameStore: Using the backend / Routes 

 * 	Completeing this project 

	*Setting up the DB with psql: 
		In order to set up the project, i created a videogames DB 
		Following, I created the tables and seeded the data within seedData.js into the db 

	*Setting up routing between index.js and the api videoGames.js file (Which uses the DB videoGames.js file)
		After setting up the DB it was time to set up the proper routing so I could work on the functionality of the express app 
		I quickly found that the layout of this express app was different compared to more novice projects I had woreked on 
		In this express app the index.js file contains the  port numbers, and is where routing to the API app occurs as well. 
		After setting up the routing, I used Insomnia to test the functionality of my endpoints. 
		The first endpoint was the hardest, It taught me that I need to rememeber to use quotation marks when creating DB's and tables 
		I spent a great deal of time wondering if my psql was working becuase I had created a DB called gamestore instead of gameStore, and a table called videogames, intstead of videoGames
		Once the issue with the casing was ressolved, and routing was implemented I was able to complete the functionality of the db/api videoGames.js files 


More information: 

Key: 
	? Issues I experienced
	* Solutions: 


	?	I had an issue with the SeedData.js file. The issue appeared to have a errorwhen running the npm run seed command. What would occur is the log would say you could run client.connect more than once. 
	
	*I found that I could manually open the psql in the terminal, and paste the code to create a table, then seed the data after the table was created. 


	? Was having an issue with creating a route 
	*
	//* Use the videoGames router for any requests to /video-games
	
	? I was using the incorrect syntax to establish the app.use within the index.js file.
		Below is the correct syntax for future reference: 
	*	app.use('/api/video-games', videoGamesRouter);

	? When creating the DB and Table in psql I didn't use " " so my casing was lowercased.  
	* 	Moving forward ensure to ues " " when creating things in the terminal as it keeps the casing of the word. 
	


? SQL : Understanding it! 

*Columns 
	Identify the data type 

	*Column Types: 

		INTEGER: Used to store integer values | 35
		FLOAT: Used to store decimal values | 0.25 
		CHAR(1): Used to store character data | x 
		VARCHAR(3): Used to store variable-length character data | abc
		DATE: Used to store date values | 1994-10-27 
		BOOLEAN: Used to store true/falsy values | TRUE 
		TEXT: used to store large amounts of text | 'This example'
		BLOB: Used to store binary data  | 0001010011000001
*Rows 
	Are the data itself 

	

*SQL Commands: 
		you can compare some of these commands to CRUD operations 

	*SELECT: used to retrieve data from a db | R in CRUD 
		
		i/e:
		-SELECT first_name | selects data from a db 
		-FROM employees | anything that returns a rowset, table, view, function, or system provided info 
		-WHERE YEAR(hire_date)=2020; | used to specify a condition while fetching the data from a single table or by joining multiple tables. 
			-This is a PREDICATE | or an expression that evaluates to TRUE, FALSE, or UNKNOWN
		

	*INSERT: used to add new records to a db | C in CRUD 
	*UPDATE: used to modify existing records in a db | U in CRUD 
	*DELETE: used to delete records in a db | D in CRUD 
	*CREATE: used to create a new table in a db 
	*ALTER: used to modify an existing table in a db 
	*DROP used to delete a table from a db 
	*TRUNCATE: used to delete all records from a table 
	*JOIN: Used to combine data from multiple tables 
	*INDEX: used to create an index on a table 


*Primary Keys 
	the primary key constrain uniquely id's each record in the table 
	Primary keys must contain UNIQUE values and cannot contain null values 
	
	A table can have one primary key, and in that table, this primary key can consist of single or multiple columns 
						*^aka (fields)

*Foriegn Keys 
	Foriegn keys are used to link two tables together in a relational databse. A foriegn key is a column or group of columns in a table that references the primary key or another table 

	Constraints: 
		SQL foriegn key constraints are used to enforce the integrity of a database. Constraints check that a foriegn key value in one table matches a primary key value in another table 


*Junction tables 
	Are used to establish relationships between two or more tables in a relational databse. 
	They are used to store primary keys of the related tables.
	*The logic here is they have FK's that connect to other tables PK's 

	Example: 
	
	*_Book Table_ 
	  Bookid(PK)-> 									-Bookid->	
	  														*_Authors Table_ 
	  Title 		***Junctional Table***                    Author ID (PK)
	  Price 		***	Junction ID    ***	                  First Name 
					*	-Book ID(FK) ->      *                    
					**********************






*Authentication 
	Is verifying a user's identity. a unique identifier is associated with a user which is the username or userid 
		A combo of username and password is used to authenticate a user 
		*JWT - JSON WEB TOKENS 
			-Are used to authenticate users in Express.js applications 
			-it is an open standard that defines a compact and self contained way of transmitting data between two parties 
			-Tokens are used to securely authenticate users in Express.js applications 
			-They are signed with a secret key, which ensure that the data is not tampered with 


			
?Json Web Token 
				Bits on encoded JSON data with cryptographic signartures at the end 
					Is the standard tool used for authorization. 
				
				*Structure of the JWT 

					*Header:
						contains info about teh algorithin and token type 
						is a 64 URL encoded, and decodes to the following JSON object: 
								{ 
									"alg": "HS256", 
									"typ": "JWT" 
								}
					*Payload
						contains the registered claims of identifying information about user... also a 64 URL encoded which decodes to the following: 
							{ 
								"sub": "1234566778" -> this is the subject of the JWT
								"name": "John Doe" -> name of user
								"iat": 	1516239022 -> issued at date for the token 
							}

					*Signature segment 
						contains cryptographic signature of token. It ensures that the data in the header and payload segments havent been tampered with and JWT can be trusted 

						

						i.e: WcPGXClpKD7Bc1C0CCDA1060E2GGlTfamrd8-W0ghBE



			Example of how JWT works:  
					1. jwt.sign assist creating a token for the user upon login with user/password payload. 
					3. Sends encrypted JWT to the client 
					4. Client saves JWT on local storage 
					5. Client sends an auth request with JWT in header 
						headers : {
							"Authoriation": "Bearer ${JWT_TOKEN}" 
						}
					6.Server compares JWT in client's header to JWT in database via jwt.verify + secret word 
					7.Server sends response on every subsequent request. However step 6 is the precursor to complying with the response to client 

		
			
		*jwt sign
				Is the proccess of generating a token that serves as a means of securely transmitting information between two parties. During sign the following occurs: 
					-Payload created, header is defined, digital signature created  
					const verify  = jwt.verify(token, secret)
					-Token is created by concatenating the parts above. 

		*jwt verify 

				Frontend (React): The user submits their login credentials (e.g., username and password) through a form.

				The server receives the login request and checks the credentials against the database (PostgreSQL). If the credentials are valid, the server generates a JWT using a secret key and sends this token back to the client.
						-Decomposition 
						-Decoding 
						-Verification of signature 
						-Claims validation: claims with the payload are examined (expiry)
				
				Frontend (React): Upon receiving the JWT, the client application typically stores it either in memory, local storage, or cookies. This token is then sent along with subsequent requests to the server to access protected routes or resources.


		*jwt decode 
				This function solely decodes the payload, it does not verify the authorization provided via the heading, signature and secr et. 


				*process.env.JWT_SECRET 
					In node process refers to a global object. 
					process.en is a property that hosts the user environment. It allwos Node.js application to access variables. 
					This ofc requires you to have password within .env 

		*Example: 

				require('dotenv').config();
				const jwt = require('jsonwebtoken');

				*Payload to be encoded
				const payload = {
				userId: 1,
				username: "user",
				isAdmin: true
				};

				*Sign the JWT
				const token = jwt.sign(payload, process.env.JWT_SECRET, { expiresIn: '1h' });

				console.log("Signed JWT:", token);

			
		*Middleware to verify the JWT

				*Aha momeent .. 
					 code resulting in just the token
					No authorization present means null 
					If I passed a jwt that I signed, it will be verified based on validity not type
					Meaning if it is the same token that I used and attached to the user, then I'm good! 
					token then gets placed into a verify with the secret jwt key 
			

					const verifyToken = (req, res, next) => {
					const token = req.headers.authorization?.split(" ")[1]; // Assuming the token is sent as "Bearer <token>"
					if (!token) {
						return res.status(403).send("A token is required for authentication");
					}
					try {
						const decoded = jwt.verify(token, process.env.JWT_SECRET);
						req.user = decoded;
					} catch (err) {
						return res.status(401).send("Invalid Token");
					}
					return next();
					};


				* Protected route example: 
					router.get('/protected', verifyToken, (req, res) => {

					Logic to handle endpoint request after verification from verifyToken

					res.send('Access to protected data');
					});



?Bcrypt 
Is a library to help with hashing passwords. It uses a password-hashing function that is based on the blowfish cipher.
		

			*Hashing
			Is converting a password into something that looks completely different from it's OG form through a mathematical algorithim
			
			*Salt Hashing 
			In the field of cryptography , actually means to add an additional string of 32 more characters to the pw before it get's hashed  



	*How to store a cryptic Password: 
		To Use Bcrypt ensure to:

			* 1. install/import the library
				npm install bcrypt
				const bcrypt = require('...")

			*2. Establish a SALT_COUNT=<anumber>
				This defines the cost or complexity of encryption can be defiend within or without parameters of b.c function. 

			*3. Create a hashedPassword from user's input 
			set the sensitive information = to use bcrypt as a async function within the parameters include both the sensitive data, and the SALT_COUNT


			const hashedPassword = await bcrypt.hash(password, 10);


			*4. Now rather than using the actual pw in SQL language for storage, you'll use the encrypted const (from step 3)
		



	*Login : comparing a plaintext password to a bcrypt one:

			This could be used in a login endpoint on the backend to verify if the user's plaintext password matches the password within the SQL db 

		i.e: 
				
			const bcrypt = require("bcrypt"); 
			const hashedPassword = " ......" 

			const plainTextPassword = "myPassword123"; 

			bcrypt.compare(plainTextPassword, hashedPassword, function(err, isMatch) => {
				if (err) { 
					console.error(err)
					return; 
				}
				if (isMatch) { 
					console.log('Passowrd is correct) 
				}
				if(!isMatch) { 
					console.log('Password is not correct)
				}
			}); 





*Authorization 
	Is verifying a user's permission. Or a process where we can allow or restrict resources to said user. 
		Depending on the business logic the requirement of user authorization can vary. 

		Basics of authorization scenario: 
			-Create  a defined role as per specific use cases 
			-extend or restrict certain roles depending on use cases
			-Assign custom actions to user to fine grain


*Dotenv 
is a worldwide standard for managing environment variables from development to production. 
1. Load 
2. Sync 
3. Deploy 

It integrates everywhere you already write, test, and deploy your code 
	? meaning it is responsible for importing the env ? into your code
		curious because i see : 
			require('dotenv').configK(); 

*Environmental Vairables 
is a variable whose value is set outside the program, Typically through functionality built into the operating sustem or microservice. 

Environmental Variables are stored as name/value pairs. Any number of these values can be created. 
	i.e: 
		NODE-ENV: developement 
		PORT: 8080
		PG_HOST: localhost 
		PG_user: happyuser123 
		Pg_password: somesafepassword 
		Pg_DB: my_happy_db 
		Pg_PORT: 5432  

(sort of what I do  with insomnia but local in the vscode workspace instead?) 
				




? Other Understandings from Block34: Juicebox 



*Postgres / Workspace Setup 

	1. Postgres is installed working at port 5432. 
	2. Login as postgres use. 
	3. Initialize the DB -
		Check the client.js or HTML file in DB directory identify the database name and port number before making the databse. 
	4. Show all databases to confirm it was built. 
		\L 
	5. Install npm packages 
		npm i 
	6. Patch errors within Seed.js -> Seed Database. 
		a. It's always a good practice to test the DB with console.logs after it's been seeded 
		b. client.end to finish this process 
	7. Set up the util.js with whatever utlitlies you want 


## Findings 

1. createInitialUsers() - function did not have enough placeholders within the index.js files causing it to stop the seeding process 

2. 

## JWT & ENV 
<!--  
*   Setting up the .env file: 

    *npm install dotenv
    install the library 

    *create a .env file in the root directory of the project
    This file will be in the root directory of the project
        *Ensure to inlcude this file within the .gitignore file 

    *call the library within the root HTML file 
    Within the root HTML file ensure to call: 
        require('dotenv').config();
    
    *How it works: 
    After this is all set, all variables within the .env will be loaded into "process.env" when the app starts giving me the ability to use it globally. 

    *How to use it 
    Whenever I want to use jwt_SECRET reference it from process.env as follows: 
        const jwtSecret = process.env.JWT_SECRET;

	*What is the best practice while using: 
		include teh following information in your .env file 
			user 
			host 
			database
			password 
			port 

 



Directory Definitions

<!--

*1. Index.js/client.js file in DB Directory:
    This file is created and exported in order to establishing a connection to the databse via PostgeSQL client library aka 'pg'. This file contains the code needed to create a client which connects to the database allowing us to execute queries and manages transactions.

*2. 'Pg'
    Is a popular way to interface with the PostgreSQL from Node.js applications.

*3. The Api directory

*       3a: Index.js
        The index.js file is an entry point for the API. It aggregates all API routes and exports them for use in the main server file (global Index.js file)

*       3b: post.js
        Contains the API routes that handle request related to post
            i.e: creating post or retrieving post

*       3c: tags.js
        Contains the API routes for "tags
            i.e: creating a tag , getting all tags etc

*       3d: users.js
        Contains the API routes for user-related actions
            i.e: registration, authentication, user profile operations etc

*       3e utils.js
        Includes the functions  that are used across different API routes
            i.e: error handling, response formatting, and middleware functions

			const requireUser = (req, res, next) => {
				res.status(401);
				if (!req.user) {
					next({message: 'you must be logged in to perfomr this action!' });
				return;
		}
			next();
  }

  module.exports = {
      requireUser
}


?Creating the Fronted


* 		1. Go to global index page and use the following code to have the fronted on the same port as the backend:
		const path = require("path");

		server.use(express.static(path.join(__dirname, "dist")));
				This will be dist if ran with vite, as vite makes a dist instead of a build directory
		*1.5:
			If that doesn'tn work you can go into vite.config.js and insert the following to change the port

				import { defineConfig } from 'vite';
				import react from '@vitejs/plugin-react';

				export default defineConfig({
				plugins: [react()],
				server: {
					port: 3000 // Change the port number to your desired port
				}
				});



*		2. go to main directory and create a vite@latest project
		npm create vite@latest
			  	cd vite-project
  				npm install
  				npm run dev

* 		3. make a build / dist folder
			npm run build

*		4. Move the dist directory into the main folder




? 	Block34A:

	* ORM
		Object Relational Mapping is a technique that connects relational databases and object oriented programming languages
			Benefits include:
				*Simplified Data Access
					Interact with DB without writing complex SQL queries

				* Object-oriented approach
					Make the code more reusable, modular, and easier to maintain

				*Supports multiiple databases
					Works the following DB's
						-MySQL
						-PSQL
						-MongoDB
							etc
				*Optimized Performance


		* Prisma
			Is an 
			
			open source database toolkit that does all of the above , making db access/manipulation seamless
		 		*Key features
					-Efficient query building and data modeling
					-Automatic schema migrations
					-Strong typing and auto-completion support
					-Databse agnostic, supporting: PQSL, MySQL, SQLite, etc.


*Understanding the PSQL / PRISMA Configuration

	*	schema.prima File:
			*this is where tables or models are defined along with the connection of the prisma file with the database.

			Configure source database in prisma schema file with information in double quotes
					"The file below doesn in a .prisma file extension
					datasource db {     -> Schema keyword
						provider = "postgresql"   -> The specifies the databse system
						url = env("DATABASE_URL")   -> PSQL url
					}

		*How  works:

				Prisma data modeling defines the data structure and relationships using its declerative language

				Prisma schema is used to define the data models and relationships in an application.

				*The syntax elements of a Prisma schema are:

					*Models
					*Fields
					*Primary Key
					*RElationshipis
					*Foriegn Key
					*Data types
					*Field Attributes


		*Prisma Schema Syntax

					datasource db {     -> Schema keyword
						provider = "postgresql"   -> The specifies the databse system
						url = env("DATABASE_URL")   -> PSQL url
					}
					*specify the client generator
					generator client {
						provider: "prisma-client-js"
						output = "@prisma/client"
					}
					*Define the data models
					model User {
						idelnt@id @default(autoincrement())
						usernameString @ unique
						email String @unique
						createdAt DateTime @default(now())
						posts Post()
					}
					model Post {
						idlint @id @default(autoincrement())
						title String
						content String
						published Boolean @default(false)
						createdAt DateTime@default(now())
						authorUser? relation(field:[authorId], references: [id])
					}


		*Prisma Migrate
			Is a schema tool by Prisma, a populate databse toolkit and ORM tool
					Schema: orginization of the database

				Prisma Migrate uses migrate files to manage and evolve the database schema
				Migration files represent changes to the database schema overtime
				Each Migration file contains operations like table creation and column modifcation
				Prisma Migrate maintains a migration history to track applied migrations


			*Key features:

				Tracks and manages databse migrations

				Generates migration files automatically based on changes to Prisma schema

				Ensures smooth evolution and data migration

				Provides rollback capability for reverting changes if needed


		*Distinguishing Prisma Client and Prisma Migrate

			*Prisma Migrate
				*think version control
				Databse Schema Migration tool
				Manages and eveloves database schema over time
				Defines schema changes using a declerative schema language
				Generates and executes SQL migration files

			*Prisma Client
				*an ORM which creates a API to interact with the db. The API adjust and updates as changes occur... Auto generated Database Client
				ORM tool
				Autogenerates a type safe API based on the schema
				Performs database operations and queries data
				Enables CRUD operations and complex queries

				*Prisma Client Operations


					*Create
					const createUser = await prisma.user.create({
						data:{
							name::"John Doe",
							email: "john@example.com"
							age:25,
						},
					 });

					 *READ
					 const users = await prisma.user.findMany();
					 const users = await prisma.user.findOne({
						where:{id:1},
					 });

					*UPDATE
					const UpdatedUser = await prisma.user.update({
						where: {id: 1},
						data:{
							age:26,
						},
					});
					*DELETE
					const deletedUser = await prisma.user.delete({
						where:{id:1},
					});
					*Closing Prisma Client
					await prisma.$disconnect();


? CLI Steps for creating a new Prisma web app 

*1 npm install -prisma --save-dev
			add the Primsa CLI as a dependency to my project


*2 npx prisma init

			-creates a new dir called prisma with file schema.prisma
			which contains the Prisma schema with databse connection variable and schema models
			-Creates a .env file in the root of the dir of my project which is used for defining env variables (datapostgresql://USER:PASSWORD@HOST:PORT/DATABASE?schema=SCHEMAbse connection)

*3 set up the schema.prisma file


			which connects the db & and defines tables

				generates a prisma javascript client
					generator client {
					provider = "prisma-client-js"
					}

			datasource db {     -> Schema keyword
								provider = "postgresql"   -> SQL type
								url = env("DATABASE_URL")   ->
								!PSQL url (is defined in .env)
							}

				? see additional notes in detail below for more info

			*connecting to the db  &&	building the URL

					Copy this sample to start:
						* postgresql://USER:@localhost:PORT/DATABASE?schema=public


						 Postico: has your username (jsjulio)
						 delete the password
						 localhost - if working locally
						 port should be in the index db doc or in env
		i.e:

	datasource db {
	provider = "postgresql"
	url = env("postgresql://jsjulio:@localhost:5432/classroom_manager?schema=SCHEMA")
	}		    connector 		baseURL 				path 				Arguments

schema=___		Arugments: The connection URL can take arguments
			For more info:
			https://www.prisma.io/docs/orm/overview/databases/postgresql#connection-url



				?Additional notes in detail:

					* prisma.schema file

							generator client {
							provider = "prisma-client-js"
							}

							define the database to connect to
							datasource db {
							provider = "postgresql"
							url      = env("DATABASE_URL")
							}

						*	model instructors {
							id Int @id @default(autoincrement())
							username String @unique
							password String?
							students students[]
							}
							Line16
							one-to-many: This line defines a o-t-m relationship which means that a single User can be associated with multiple post
											In other wors , each user has a list (array) of post

				*			model students {
							id Int @id @default(autoincrement())
							username String
							password String?
							author instructors @relation(fields: [authorId], references: [id])
							authorId Int
							}

					*		Line24:
							author: this declares a field named author on the Student model":
								this field has a type of 'instructors' allowing it to reference the Instructors model
							relation: This is a prisma decorator used to specify that the field is in relation between models
							fields: This specifies the COLUMN in students model that serves as the foriegn key for the relationship
							references: inidicates that the authorId field on students refers to the id field on instructors
											so authorId is a FK that references the id on User
								*when it is suggested to use lowercase models to be compliant with symantics
								*as well as ausing author / authorid within child models to semantically refer the parent model



						*5 npx prisma migrate dev --name init
							Creates the DB with defined models(Tables) that are in the schema.prisma file
							?Run this code if you want to restructure the db (Add more rows or columns)
							?Followed by npx prisma generate 

						6 FYI : reintegrating all files with Prisma



						api directory
							prisma will not replace this file since it handles the routing, response formatting. Instead Primsa will be integrated into these routes to do db ops

						db directory
							Prisma will replace the db folder's functionality. UNLESS the db folder contains logic that is not directly related to ORM ops such as databse utiltiies, or custome SQL quieries that Prisma cannot handle.

						*7.npm install @prisma/client




? Steps for creating prisma with an exsisting Database
This means that your database is seeded with working SQL logic already
https://www.prisma.io/docs/getting-started/setup-prisma/add-to-existing-project/relational-databases-typescript-postgresql



	*1. npm i --save-dev prisma@latest
		install

	*2 npmx prisma init
		explination same as shown above

	*3. set up the schema.prisma file

			modify the datasource
				As shown above

			modify the URL
				As shown above

	*3.5
		If you do not have a seed.js from PSQL you can use the prima version of seeding a database: 
		*a.create the seed.js file 
				const { PrismaClient } = require('@prisma/client');
				const prisma = new PrismaClient();

				async function main() {
					/ Deleting existing data
					await prisma.player.deleteMany({});
					await prisma.game.deleteMany({});

					/ Creating a new game
					const game = await prisma.game.create({
						data: {
						/ Add game-specific fields if needed, e.g., status: 'active'
						},
					});

					/ Creating players with initial data
					const playerData = [
						{ name: 'Player 1', lives: 3, inGame: true, gameId: game.id },
						{ name: 'Player 2', lives: 3, inGame: true, gameId: game.id },
						/ Add more players as needed
					];

					for (const player of playerData) {
						await prisma.player.create({
						data: player,
						});
					}

					console.log('Database has been seeded.');
					}

					main()
					.catch((e) => {
						console.error(e);
						process.exit(1);
					})
					.finally(async () => {
						await prisma.$disconnect();
					});
				
				/ Creating a new game
				const game = await prisma.game.create({
					data: {
					/ Add game-specific fields if needed, e.g., status: 'active'
					},
				});

				/ Creating players with initial data
				const playerData = [
					{ name: 'Player 1', lives: 3, inGame: true, gameId: game.id },
					{ name: 'Player 2', lives: 3, inGame: true, gameId: game.id },
					/ Add more players as needed
				];

				for (const player of playerData) {
					await prisma.player.create({
					data: player,
					});
				}

				console.log('Database has been seeded.');
				}

				main()
				.catch((e) => {
					console.error(e);
					process.exit(1);
				})
				.finally(async () => {
					await prisma.$disconnect();
				});


*			b.install the Prisma Client (see step 5)
	*		c.add a seed command within the package.json scripts 
				"scripts": {
					"seed": "node prisma/seed.js"
					}
			*OFNOTE: 
				-make sure to create a development and production environment. Do this by manipulating the code within package.json : 
				-from this 
					"scripts": {
						"dev": "parcel index.html --no-cache --config ./parcel/.parcel.dev --open",
						"build": "parcel build index.html --public-url _relativeroute_ --no-source-maps --log-level error --config ./parcel/.parcel.prod"
					},
				-to this: 
					"scripts": {
						"dev": "NODE_ENV=development parcel index.html --no-cache --config ./parcel/.parcel.dev --open",
						"start": "NODE_ENV=production node server/index.js",
						"build": "NODE_ENV=production parcel build index.html --public-url _relativeroute_ --no-source-maps --log-level error --config ./parcel/.parcel.prod",
						"seed": "node prisma/seed.js"
				},
			
				then make your seed.js file only run within development by running this code at the beginning 
					if (process.env.NODE_ENV === 'production') {
						console.log('Seeding is not permitted in production!');
						process.exit();
					}


	*4 npx prisma migrate dev --name init
		Creates the DB with defined models(Tables) that are in the schema.prisma file
		?Run this code if you want to restructure the db (Add more rows or columns)
		?Followed by npx prisma generate 


	*5  npx prisma db pull
		TODO Whenever you clone a project with prisma, you start here. 
			Which makes sense, you need the env files to operate the project 
		? If it is your own project copy the env file over, if not, create one. 
		WALLAH! 

		This commmand is dope! It read the Database_URL (located in the .env) and connects to the db following. It then introspects the database & translates the database schema from SQL into a prisma data model

		To get the latest prisma run:
			
			

	*6 npm i @prisma/client@latest
		this command creates a node module which houses the prisma client. That node module is changed evertime the schema is modified but in order to change it you have to run the following: 

		*7 npx prisma generate
			This reads the prisma schema and generates my prisma client library within the @prisma/client node_modules


	*8 set up the enviornment and do you first prisma quiery

		*a. Import Prisma Client
		const { PrismaClient } = require('@prisma/client)
		const prisma = new PrismaClient()

		*b crud methods can be found here:
		! https://www.prisma.io/docs/orm/prisma-client/queries/crud



?DOPE PRISMA understandings:

	*jwt.sign
		occurs whenever a authenication occurs. So during registration and login , you'll see a jwt function

	*jwt.verify
		jwt.verify() is a method provided by the jsonwebtoken (JWT) library in Node.js. It is used to verify a JWT's signature and optionally its claims (like expiration, issuer, audience, etc.).

	*To create new models:

		add them to the prisma.schema file then run:
			npx prisma migrate dev --name <modelname>-model

	*use Auto complete to learn about different API calls
		CTRL + SPACE

	*You can manually change the database schema with seed.js then

		re-introspect to reconfigure the prisma.schema file then

		reconfigure the prisma client libraby

	*npm run server
		to start server for both the DB and front-end

	*"server:dev": "JWT=JWT node --watch server",
		This script sets an environment variable JWT equal to JWT and starts the server with '--watch' which automaticall restarts the server when a file changes .


	*place shutdown logic within the index.html file that is in the root of the server:


	*prisma 








? Block34B: Authentication and OAuth 

	*GOALS
		learn how to use Bcrypt to encode passwords 
		Authenticate users using Github and OAuth 
		




	?Authentication using Bcrypt 
	Is verifying a user's identity: username/pw

		*JWT - JSON WEB TOKENS 
			-Are used to authenticate users in Express.js applications 
			-Tokens are used to securely authenticate users in Express.js applications 
			*JWT signs 
				are signed with a secret key, which ensures that the data is not tampered with 


		*Bcrypt 
			Is a library to help with hashing passwords. It uses a password-hashing function that is based on the blowfish cipher.
				*Hashing
					Is converting a password into something that looks completely different from it's OG form through a mathematical algorithim
					*Salt Hashing 
						In the field of cryptography , actually means to add an additional string of 32 more characters to the pw before it get's hashed  


	?OAuth : what is it? 
		is an authorization framework that 
			*enables a webiste or application to use resources from other web apps on behalf of the user 


		Roles within OAuth: 
			-Resource owner 
			-Client 
			-Authorization server 
			-Resource Server 
		
		Exploring OAuth: Accesssing delegation and Authentication 
			1. Initial Request 
			2. Authorization grant 
			3. Authorization code 
			4. Token Request 
			5. Token Response 
			6. Resource Access 
			7. Token expiration and refresh 

			
		?Steps to setting up OAuth: 

			*1. Set up a Github OAuth application 
				Settings > Dev settings > OAuth apps > New Github app 
			
			*2. GitHub redirect back to my site 

			*3 Use temporary code to get an access token 
				{ 
					access_token="YOUR_ACCESS_TOKEN", 
					"token_type": "brearer"
				}
			*4 Get the authenticated user 
				{ 
					GET https://api.github.com/user
					Authorization: token YOUR_ACCESS_TOKEN 
				}


*34B Guided Practice helpful tips ? 

			1. create an arrow function using app.get method. Pass the /auth/github/callback,req, res as parameters in the arrow function and store the value of req.query.code to the code variable.

			App.js: 
				const express = require("express"); 

				const app = express(); 

				app.get("/auth/github/callback", (req, res) => {   const code = req.query.code; }); 

				app.listen(3000, () => { 

				console.log("Server is running on port 3000"); 

				}); 

	*2. Write a two line code that uses bcrypt to hash the password with 8 salt rounds 
			
			const bcrypt = require('bcrypt)
			const webTextPassword = "Password" 
			const hashedPassword = await bcrypt.hash(webTextPassword, 8);


		3. Wite a line of code in JS that makes a Post request to exchange the authorization code for an access token in Github OAuth 

	*4. Create a line of code that switches the authorization logic for an access code token in GitHub OAuth 

			const axios = require("axios");
			const response = await axios.post(
			"https://github.com/login/oauth/access_token",
			{
				code: "AUTHORIZATION_CODE",
				client_id: "YOUR_CLIENT_ID",
				client_secret: "YOUR_CLIENT_SECRET",
				redirect_uri: "YOUR_REDIRECT_URI",
			}
			);


?Block34B Bcrypt and OAuth 

	Goals of assignment: 

		This criterion is linked to a Learning Outcomebcrypt bcrypt is used to encrypt a user's password before it is sent to the server.	

Rubric 
		*Frontend components are updated to signify the "Login via Github" option.


		*A redirect route has been added to the backend to receive the authorization code from Github.
			callback URI which 
				-GitHub sends temporary query parameter on url  which youll use to do a server to server post 
				-server to server post: to github access token URL 	
					which takes temp code and app's client secret to request user access token 

		*The backend is able to make requests to Github on behalf of a user by sending an access token.
				server send tokent to client application (As a cookie) to maintain logged state and complete request 
				

		*The account for a user logged in via Github is created and stored in the database.
				

		*The client still receives a token from the server after a user is successfully authenticated, regardless of whether the user logged in via Github or username/password.





	?Bcrypt What I know:  



		Bcrypt 
		Is a library to help with hashing passwords. It uses a password-hashing function that is based on the blowfish cipher.
				

					*Hashing
					Is converting a password into something that looks completely different from it's OG form through a mathematical algorithim
					
					*Salt Hashing 
					In the field of cryptography , actually means to add an additional string of 32 more characters to the pw before it get's hashed  



			*How to store a cryptic Password: 
				To Use Bcrypt ensure to:

					* 1. install/import the library
						npm install bcrypt
						const bcrypt = require('...")

					*2. Establish a SALT_COUNT=<anumber>
						This defines the cost or complexity of encryption can be defiend within or without parameters of b.c function. 

					*3. Create a hashedPassword from user's input 
					set the sensitive information = to use bcrypt as a async function within the parameters include both the sensitive data, and the SALT_COUNT


					const hashedPassword = await bcrypt.hash(password, 10);


					*4. Now rather than using the actual pw in SQL language for storage, you'll use the encrypted const (from step 3)
				



		*Login : comparing a plaintext password to a bcrypt one:

					This could be used in a login endpoint on the backend to verify if the user's plaintext password matches the password within the SQL db 

				i.e: 
						
					const bcrypt = require("bcrypt"); 
					const hashedPassword = " ......" 

					const plainTextPassword = "myPassword123"; 

					bcrypt.compare(plainTextPassword, hashedPassword, function(err, isMatch) => {
						if (err) { 
							console.error(err)
							return; 
						}
						if (isMatch) { 
							console.log('Passowrd is correct) 
						}
						if(!isMatch) { 
							console.log('Password is not correct)
						}
					}); 





? 	GitHub Apss vs OAuth Apps:

*OAuth defined: 
OAuth allow for users to let servers read their data and provide a function, without ever having to create an account on the server... users do not need to actually share credientials 

	*In the context of 34B: 
		GitHub's OAuth 2.0 flow allows users to grant my application to access their GitHub data without them having to share a GitHub password with my application. As a result I authenticate users that use my application while leveraging github as the identify provider. 
	
	*Workflow of the exhange: 
		Users:	 users log into github, authorize my app, and install my app. By installing my app on their account, they grant the app perimssion to access the orginzation and repository resources that they requested




			*OAuth flow steps Try 1: 




				*Creating a GitHub app quick starter 
					https://docs.github.com/en/apps/creating-github-apps/writing-code-for-a-github-app/quickstart

				 Writing the code for the GitHub login button
					 https://docs.github.com/en/apps/creating-github-apps/writing-code-for-a-github-app/building-a-login-with-github-button-with-a-github-app

				Creating a authentication access code: 
				 	https://docs.github.com/en/apps/creating-github-apps/authenticating-with-a-github-app/generating-a-user-access-token-for-a-github-app 


				1. Client arrives to me app login page 
				2. Client gets pushed to the authorization URL 
						This url is on GitHub's domain and includes query parameter such as the client_id or my app? and the redirect uri (my callback URL) and any scope parameters that determine teh level of access my app is requesting. 
							example: 'https://github.com/login/oauth/authorize?client_id=...&redirect_uri=...&scope...' 
						This endpoint handles the exhange or temporary code recieved from Github for an access token. 
				
				3. GitHub page: Client gets pushed to the Github page that will ask them to log in and or authorize the web app. 
				
				4. After this client logs in authenticate with GH, Github redirects them to my app via the"redirect_uri" portion I specified, and appends a temporary code as a query parameter. 
						Example: https://yourapp.com/callback?code=temporary-code


				5. Backend exhanges this temporary code for a access token. This is done by a server to server POST request to GitHub's access token URL, sending along the temp code and my applications client secret

					server to serverpost uses the client secret and the private key to verify thay my app is who it says it is


				6. GitHub responds to my server with an access token if the code exhange is successful 

				7. My apps client Side: My server sends this access token to the client application, often setting a sesion cookie to maintain the user's logged in state. 

		
				8. My app then allows users to create an instructor account without requring them to fillout a registration form. Intead the app can now operate on the user's behalf since the account is granted said permission from user. 



?OAuth Steps try 2:  

		*0. Forked the project and set up a env file and set up Prisma Schema

	*		0.5 Ensured env / .gitignore files were set up well 
					1 .gitignore

					1 .env's : one in client 
						Just place client_id in auth.jsx 

							-.env
								# dotenv environment variable files
								.env
								.env.development.local
								.env.test.local
								.env.production.local
								.env.local

					When needing to update the client app, npm run build was required since app was in the dist directory 

		* 	1. Created a GitHub App link button with onClick / handleOnclick event/function on Login Component

			handleClick func - redirect user to GH too authenticate my app 

				linkToGHAuth? client_id=${client_id}& redirect_uri=${redirect_url}

				-GHAuth Link does not change:	https://github.com/login/oauth/authorize 
				-client_id: to be defined in jsc file and retrieved from GitHubApp settings
					!ensure to use the "Iv1." portion of the code! 

				-redirect_uri: where user will be redirected and see a loading page while follow on server to serveer CRUD operations occur 
						(Link is the same as endpoint/ "Callback URL" on GH) 

						Failed GitHub code response: http://localhost:3000/auth/login/github/callback?code=8ea3a4e98fb3afcdac49 
							*8ea3a4e98fb3afcdac49
							
						Successful git hub code response:  http://localhost:3000/?code=62dc4b44177ed704798f
							*62dc4b44177ed704798f

		*2. Added updates to the app to Reach Auth 
				ensure to use the "Iv1." portion of the code! 
				place client_id in the auth.jsx component


		*2.5 Recreated the prisma.schema to have a boolean identifier: isGitHub
				boolean is by default false, and only true if you create with GitHUB

		*4. Modified my schema so that it can track when a user if a GitHub user 
		created an optional boolean that is by default false/ 


		*5.Successful in updates and proceeded to handle server logic to create players 


			*At the uri  endpoint the goal is for my server to make a POST request on GitHub's access token endpoint ... The body of the request provides the following vital data: 

				App client_id, 
				client_secret, 
				and code (attached onto callback url sent from GH) 
						http://localhost:3000/auth/oauth-callback?code=981c691785406cc0b4ba
							curent code 981c691785406cc0b4ba

			Create logic to make a post ^ 


			The access token is then used to make a GET request to GitHub's user endpoint to retrieve the user's username and id
			The user's username and id are then used to check if the user already exists in the database

				If the user doesn't exist, a new user is created in the database
					ensure to add true to isgithubuser in the create user function within this endpoint
				A JWT token is then signed for the user and sent to the front-end app
				The user is then redirected to the front-end app with the token
				The token is then stored in the front-end app's local storage
				The user is then authenticated and can access protected routes
				If the user already exists, a JWT token is signed for the user and sent to the front-end app
				The user is then redirected to the front-end app with the token
				The token is then stored in the front-end app's local storage


	*Different type of tokens and their use: 
	

			*Installation access tokens
				are used to make API requests on behalf of an app installation.
				for apps that run in conjunction with my server 
				require a private key
				attribute activity to my app: 
					useful for automations that act independently of user 

			*User access tokens 
				are used to make API requests on behalf of a use
				are for client side applications that run on user devices and not on my server.
				attribute activity to users and app 
					 useful for taking actions based on user input or on behalf of user

			* Refresh tokens 
				are used to regenerate user access tokens
					stored in different place from active access tokens 

		*User access tokens 
			type of OAuth token that only has permission that both the user and app have. 
			-access tokens are granted access to specific repos, 
			-tokens can be revoked via the user 
		
		

	*Whatis a webhook app: 
		Enable you to automatically do something based on data
			A URL connnects two applications... When an event happens on the trigger application(GiutHub) this set up  serializes data about that event and sends it to a webhook URL from the action application... The Webhook URL leads to a server that accepts the payload and does something with the information. 

	*What is a GHA(GitHubApp) 
	Tools that extend GitHub's functionality. 
	GHA grant github the ability to automate processes. 
		*GHA's are preferred to OAuth apps becuase it's security level is more intact since GHAs mitigate damage in the case of a leak by specifying which repositories their apps can/cannot access and creating shorter lived tokens 

	*What exactly does GHA allow for? 
			- build / share apps with the community. 
			-manage projects
			-integration of APIs and webhooks into GitHub
			-customizing GitHub workflow by enabling GitHub to autonomously: 
				-open issues
				-comment of PR, 
				-complete things outside of Github : i.e: like posting on Slack when an issue arises. 

				*Concept of GitHub Apps 
					can take actions on behalf of the user OR act independently of the user. 
						This benefits the automations that do not require user input. 
			So What: 	The app will continue to work even if the person who installled the app on an orginization leaves the org 
				
						*GitHub OAuth 2.0 
							-is a type of GitHub App that can use OAuth 2.0 to generate a type of OAuth token(user access token) and take actions on behalf of the user.


	*GitHub Apps vs OAuth Apps 

				*ratelimit
				max number of API request 
				an app can make to Github's 
				servers in a given time frame

		*GHAs 
		rate limit for using access tokens are scaled as limit increases with number or repos/orgs connected
		apps have built in centralized webhooks MEANING: 
														*once an app is given permission to access a repo/org in can recieve webooks from all repos it has access to. (scalable)

		*OAuth apps 
		rate limits do not scale and are set
		requires individual configuration of webhooks for each repo and org. 
																			*tailored more for specific user authentication and authorization vs integration across multiple reops/orgs (not scalable)


? 	Creating a GitHub App: 


	*1. Register the app 
		visit: 	https://docs.github.com/en/apps/creating-github-apps/registering-a-github-app/registering-a-github-app










*Useful links / information 



		?[Building a Login/Auth button for client GitHub Authentications]
			(https://docs.github.com/en/apps/creating-github-apps/writing-code-for-a-github-app/building-a-login-with-github-button-with-a-github-app)

		*Registering a GitHub App 
		https://docs.github.com/en/apps/creating-github-apps/registering-a-github-app/registering-a-github-app


		*Registering a GitHub App 
		https://docs.github.com/en/apps/creating-github-apps/registering-a-github-app/registering-a-github-app


		*The [Quick starter guide with instructions on how to build a GitHub App]
			(https://docs.github.com/en/apps/oauth-apps/building-oauth-apps/differences-between-github-apps-and-oauth-apps)

		*[Generating a user access token]
			(https://docs.github.com/en/apps/creating-github-apps/authenticating-with-a-github-app/generating-a-user-access-token-for-a-github-app)

		*[Deploying web apps to online servers ]
			(https://docs.github.com/en/apps/creating-github-apps/writing-code-for-a-github-app/quickstart#deploy-your-app)


		*authenticating device flow 
			App sends your phone or email a code, which user enters to get authenticated 
			https://docs.github.com/en/apps/oauth-apps/building-oauth-apps/authorizing-oauth-apps#device-flow


	*	Understanding GitHub Apps and OAuth / permissions & access / Token based identification 
			https://docs.github.com/en/apps/oauth-apps/building-oauth-apps/differences-between-github-apps-and-oauth-apps


		Adding GitHub App managers: 
			https://docs.github.com/en/organizations/managing-peoples-access-to-your-organization-with-roles/roles-in-an-organization#github-app-managers


	*?Using cookies for JWTs 

		set up the middleware to also check the cookies 
			

			*Check requests for a token and attach the decoded id to the request
			app.use((req, res, next) => {
			const auth = req.headers.authorization; //auth = Bearer+token
			const tokenFromHeader = auth?.startsWith("Bearer ") ? auth.slice(7) : null; 

			let tokenFromCookie = req.cookies.token;
			if (tokenFromCookie && tokenFromCookie.startsWith('Bearer ')) {
				tokenFromCookie = tokenFromCookie.slice(7);
			}

			const token = tokenFromHeader || tokenFromCookie; 

			try {
				req.user = jwt.verify(token, process.env.JWT);
			} catch {
				req.user = null;
			}

			next();
			});

			*res.cookie("token", 'Bearer ' + token, { httpOnly: true, secure: false });
	
	
			Add "Bearer " to middleware ? 
			This code sets a cookie named "token" with the value 'Bearer ' followed by the JWT token. 
	
			The httpOnly option is set to true to prevent client-side JavaScript from accessing the cookie, which helps mitigate cross-site scripting (XSS) attacks.	

*Extracting tokens from cookies 

		const cookies = document.cookie.split('; ');
		const tokenCookie = cookies.find(cookie => cookie.startsWith('token='));
		const token = tokenCookie ? tokenCookie.split('=')[1] : null;
				
		*This code splits document.cookie into an array of cookies, finds the cookie that starts with 'token=', and then splits that cookie into a name and a value. The value of the cookie (which is the token) is then stored in token.
		
		
		The secure option is set to false, which means the cookie will be sent over HTTP as well as HTTPS. 
		
			*In a production environment, you should set secure to true to ensure the cookie is only sent over HTTPS

	*JSON secretOrPrivateKey error: 


GitHub Pilot: 
	The error message "secretOrPrivateKey must have a value" is coming from the jsonwebtoken library. This error typically occurs when you're trying to sign a JSON Web Token (JWT) but the secret key is undefined or an empty string.

	In your case, the error is happening at line 35 in the server/auth/index.js file. Without seeing the actual code, it's hard to say exactly what's wrong, but it's likely that the secret key you're using to sign the JWT is not being correctly loaded.

	Here's a common scenario that could cause this issue:

	In this case, if JWT_SECRET is not set in your environment variables, secretKey will be undefined, and you'll get the "secretOrPrivateKey must have a value" error when you try to sign a token.

	To fix this issue, make sure that the secret key is correctly defined and loaded. If you're loading it from an environment variable, make sure the environment variable is set. If you're defining it in your code, make sure it's not undefined or an empty string.

		*Fix:  
			how the app.js(in this case) mentions the secret is how you create the secret in .env




 
*Define the LinkedList class
class LinkedList {
    The constructor is called when a new LinkedList is created.
     It sets the head of the list to null, indicating that the list is initially empty.
    constructor() {
      this.head = null;
    }
  
     The insertLast method is used to add a new node to the end of the list.
     It takes one argument, the data for the new node.
    insertLast(data) {
      Create a new Node with the given data.
      let newNode = new Node(data);
  
      If the list is empty (i.e., the head is null), set the new node as the head of the list.
      if (!this.head) {
        this.head = newNode;
      } else {
        If the list is not empty, start at the head and traverse to the end of the list.
        let current = this.head;
        while (current.next) {
          current = current.next;
        }
        Once the end of the list is reached, set the next property of the last node to the new node.
        current.next = newNode;
      }
    }
  
    The remove method is used to remove a node with a specific data value from the list.
     It takes one argument, the data value of the node to be removed.
    remove(data) {
       If the list is empty, there's nothing to remove, so return.
      if (!this.head) {
        return;
      }
  
       If the head node is the one to be removed, set the head to the next node in the list.
      if (this.head.data === data) {
        this.head = this.head.next;
        return;
      }
  
       If the head node is not the one to be removed, start at the head and traverse the list,
       looking for a node whose next node has the data value to be removed.
      let current = this.head;
      while (current.next) {
        if (current.next.data === data) {
          * Once such a node is found, set its next property to the node after the next node,
          * effectively skipping over the next node and thus removing it from the list.
          current.next = current.next.next;
          return;
        }
        current = current.next;
      }
    }
  } 













--------------------


? FEB 26th | Linked List | Eliott  

*Linked List 
	-Are Data structures whose order is not given by their physical placement in memory.
	-Instead, each element points to the next. 
	-It is a data structure consisting of a collection of nodes
	-which together represent a sequence


	*Visual: 

		a linked list is a linear collection of data elements 
		stored in sequential order with: Pointers 
			*  (HEAD) ->     DATA  ____next______ DATA   ___next___ DATA _____next___ (TAIL)
							'100'	 pointer     '200'	   		   '300'				NULL
						Element/node				
			

			*Nodes
				divde into two parts: 

				*Data: Contain information on the node 

				*Poionters -> Have information on the following node 


				class Node {
					constructor(data, next = null) {
						this.data = data; // The data the node holds
						this.next = next; // Reference to the next node in the list
					}
				}















































? ALGO


	?	Linked List 


*	Theoretical Structure of linked list 
		Linked List are useful because with data storage, they allow for use of memory efficiently. 
		
		Composed of Head(Null value), Nodes + pointers (located in nodes). 


*	Nodes
	are composed of two things, a value and a pointer. In linked list, Nodes as a result of having two sets of info, take two back to back slots. First one holds the value, the memory slot points to whatever other node. 
		
		-head: the first and only defined value of the linked list. You start here to be able to traverse the entire linked list and find a certain number within list
		-Value: 
		-Pointer:  



Different data structures have different space-time complexities. Being familiar with all data structures will allow you to use the best ones to ressolve interview questions 







	?Algorithms and Analysis


	*BigO Notation 
		A way to describe the efficientcy of an algorithm as the input size grows 
			Determining how good an algorithim resolution is by determining it's Space-Time complexity 
	
		*O(n)
			-O: is defined as the order of complexity 
			-n: number of inputs


			*Time Complexity: 
				how long does it take the algo to run as time progresses 

			*Space Complexity: 
				how much memory or space an algorithim uses. Less memory is good. 

					Types of memory include:
						Bounded Canvas: Which has a predefined number of slots 
				
		*The BigO scenarios 

			* O(1)
				Contact time: Is when you get an element through it's index. Regardless how big the array is, thhis will consistently be the same 

			* O(n) 
			Linear Complexity: here the function's time span varies based on how long the arr is. It can take a while 
				i.e: A loop oover an array of element. 

			*O(Log N) 
			Logarithmic complexity
				you are able to jump back and fourth through a set of information 
					i.e: Logarithmic search :t works by repeatedly dividing in half the portion of the list that could contain the item, until the possible locations are reduced to just one. 

			*O(n^2)

			*How memory storage works: 
					-Data is stored in memory slots in the form of base2/binary bytes (which is 8 bits of 0s and 1s)
					-Program always stores variables in a series of memory slots that is free
					-If program needs more than one memory slot to store info, it'll be stored in back to back slots 
						*	fix width int(integers): 32 bits / 4 bytes 
					-you can reference the memory address of another memory slot in order to "Point" to another memory slot 
					-Accessing information from memory slots is a uncostly type of operation. 


 ? 	Bubble Sort 
		An Algorithim that loops through an array of elements in order to sort the algorithims 

		How it works: 
		Loops through elements and swaps out anything that is out of order

		Bubble sort could be O(n) : if there is an array that is already sorted ..... 
			best case scenario is there is only one thing out of order 
		
			HOWEVER since we think worst case scenario, it will be O(n^2)

? Merge Sort (going over next week!)


	11MAR: 

*Merge sort
	n * log(n)
		
		this function is a two step process of 
			-taking an array and sorting it 
			-and remerging information. 
		
		It is faster than bubble sorting but because there are so many new arrays created = it is more space complex
	
		
		split things down to individual elements, then recombine them. 
		
		When recombined into sorted pairs, we then recombine into quads

		
		tricky question with this topic: how many times do we need to recombinate 
			Anwser: 
				-find the amount of levels or iterations that is required to recombine the array. 
				-round up on the log 
					O(n * log(n))

				Of note: can be completed iteratively , however not reccomended. 
*Recursion: 



/ Write a function "reverseString" that takes a string as input, and returns that string reversed. You MUST use recursion for your answer. Any form of looping (including built-ins like .forEach) are forbidden for your solution.

		*Given: 

			const reverseString = (inputString) => {   
				/ TODO
			}

			console.log(reverseString('hello')); // => olleh

			const reverseString = (inputString) => {   
				/ TODO
			}

			console.log(reverseString('hello')); // => olleh


		*Coipilot Solution: 

			const reverseString = (inputString) => {
			// Base case
			if (inputString.length === 0) {
				return "";
			}
			
			// Recursive case
			const firstChar = inputString[0];
			const remainingChars = inputString.slice(1);
			return reverseString(remainingChars) + firstChar;
			}

			console.log(reverseString('hello')); // Output: olleh




		*Eliot's Solution
		const reverseString = (inputString) => {
			/ Base Case: Return nothing if there are no characters left.
			if (inputString.length === 0) {
				return '';
			}
			/ Recursive Case: Reverse every character in the string besides for the first one.
			const restOfStringReversed = reverseString(
				inputString.substring(1, inputString.length),
			);
			/ Because, we will append whatever the "first" character was at this level to the end of the rest of the string reversed.
			return restOfStringReversed + inputString.charAt(0);
		};
		console.log(reverseString('hello')); // => olleh







? 		Final Project 


for (let team of baseballTeams) {
  // code here
}






-->
