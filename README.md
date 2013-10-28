**To add a new project to the site:**

1. Add this to /index.html:

	`<div class="project">`
	
	`{% include homepage_picturefill.html file="DIRECTORY_NAME_OF_NEW_PROJECT_HERE" %}`
	
	`<div class="info">`
	
	`<p>/03</p>`
	
	`<p><a href="apocalypse">PROJECT_NAME_HERE</a></p>`
	
	`<p>Colors Magazine</p>`
	
	`</div>`
	
	`</div>`

2. Add a new project folder contaiing the appropriate images and an index.html file. The images you need will depend on which layout you choose. The front-matter of the html file specifies the following;

	* layout: Choose from the layouts in /_layouts. Each layout shows a different number of images
	 
	* title: This appears on the project page itself
	 
	* index: As does this
	
	* client: And this
	 
	* description: Put your project description text here

**testing**

there's a basic visual test setup so you can compare visual output from youe local jekyll server and the live code on github pages. it's using Wraith from the BBC: [https://github.com/BBC-News/wraith
](https://github.com/BBC-News/wraith)

to use:

* cd wraith
* bundle
* rake

this will run Phantom, take screenshots of both local and remote sites (defined in /wraith/configs/config.yaml) and save them in /wraith/shots. Open the gallery.html file in that directroy to inspect the results of your test.