# Hosting a Static Site on GitHub Pages

The purpose of this README is to show you how to both create and upload a resume formatted in markdown onto GitHub pages using a static site generator. The resulting site will have a few features, the prominant one being that we won't need to write any XML or HTML/CSS, the other features are easy to change themes and a fully responsive site. A responsive site is a site that changes it's features to maintain a good visual appearance on multiple screen sizes.

## Some Prerequities

Before we get started, we need to get a few things set up. First we need to create a [Github](https://github.com) account if we don't already have one. After that we will need to make a resume formatted in markdown. In order to get this setup, you will first need to convert your current resume, or build a new one in markdown, if you don't know how to write in markdown, then refer to the "More Resources" section where I have linked a markdown cheat sheet and a tutorial on how to write markdown.

Next we will need a markdown editor to write our markdown in, this will be used to create both your resume and the content of any other pages you may create. I have put a link to a website in the "More Resources" section that lists a few great markdown editors, the editor I used is Byword, a paid app for the mac.

Finally, we can optionally set up Jekyll on our local machine. Jekyll is a static site generator that converts our markdown into HTML and CSS and prepares our site. [Here](https://jekyllrb.com/docs/installation/) is a tutorial on how to set up Jekyll on your machine. Developing your site locally will allow you to see your changes take place almost instantly, meanwhile, simply comitting your changes to GitHub may result in a delay of up to 30 minutes before your changes take effect.

## Instructions

1. To start with, we need to set up our GitHub Pages repository. in order to do this, we will need to open GitHub and sign in. Then, we will click the "+" button in the top right hand corner of the screen and click on "New repository". In the repository name field, type (your_user_name).github.io, the your_user_name needs to match the user name to the left of the "/" exactly. Everything else can be left as their default values, and press the "create repository" button. The Github repository is a form of a distributed version control system or DVCS for short, as mensioned by Etter in his book Modern Technical Writing;
> DVCS have better performance, allow for offline work, and are superior for concurrent work on the same file.
Though not completely relavent to this task, knowing the many features of DVCS help when working on projects in a group, as well as aid in building your site more effectively.
2. From this page, along the top bar is a settings button, click that button, and on the following screen click on the pages tab in the navigation bar on the left. Here we can click on the choose theme button, and select a theme for our website, in my case, I chose to use the slate theme. As mensioned in Etter mensions in his book 
> you provide a static site generator with content (lightweight markup) and a theme (templated HTML and CSS), and it processes everything into a working website.
In other words, Jekyll takes as input the theme and markdown, and outputs a site built with HTML and CSS.
3. After selecting a theme, go to the code tab towards the left of the screen.
4. From here we will switch to our resume. If you already have one formatted in markdown, then rename the file to index.md, otherwise, make a new file and create your markdown resume, as mentioned in the previous step, this file will be the markdown input to Jekyll.
5. Now returning to GitHub, from the code page of the GitHub pages repository, open the add file drop down and click upload files, then drag and drop index.md into the designated area, add a title for the commit, and optionally, add some comments, them press commit changes, these commits are what allow many individuals to contribute to a project, and these commits need internet, thus any progress can be stored locally until internet is present, where the commit can take place. This is directly related to how DVCS work as menstioned in part 1.
6. It can take time for changes you make to become visible on your GitHub pages site, this delay is caused by GitHub. The best way to bypass this wait interval is to develop your site locally with Jekyll until the results are satisfactory, and then commit the final result. When testing locally, Jekyll will make a local web server to host your site, as Etter mensions,
> You can test static websites on your local computer without installing anything and compress and ship them with software applications.
Simply put, there is no need to build your own web server, or download a heavy web server to test your site, and the primary benefits of doing so would be less storage usage and close to live updates on your site for each change you make.
7. Finally, to view your now completed site, on your web browser, search up your_user_name.github.io, this is the home page of your GitHub pages, and here is where you will find your resume. If you would like a reference, take a look at the "More Resources" section where I have linked my own GitHub pages site, on the site I have my resume uplaoded. 

The result of following the above steps is a site containing your resume. Below is a Gif of my resume that I have hosted on my GitHub pages.

![Gif of my resume](https://github.com/diddy5436/diddy5436.github.io/blob/main/Animation.gif)

## More Resources

A few resources on markdown:

- [Learn Markdown](https://www.markdowntutorial.com)
- [A Markdown Cheat Sheet](https://www.markdownguide.org/basic-syntax/)

[Here](https://www.oberlo.ca/blog/markdown-editors) is a website that has a list of great markdown editors, it includes the one I used, Byword, as well.

Here is my [resume](https://diddy5436.github.io) for reference.

Here is a link to [Etter's book](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS), it is a great resource to learn about markdown as well as useful information on writing technical works.

## Authors

This repository was entirely developed by me, any work that was not my own has been noted and any necessary links to my sources have been provided.

## Acknowledgements

The template I based this README off of was made by Purple Booth and can be found [here](https://github.com/PurpleBooth/a-good-readme-template).

## FAQ

#### Why is Markdown better than a word processor?

A word processor's main funtion is to create PDFs, however, in many cases, we don't want to simply download our information as a PDF, we want something that can continue to change, and also have a variety of ways to represent the information. With markdown, we can represent our information in simple text, slide shows, and websites. There are many more ways of presenting markdown, which makes it far superior to a word processor in many areas.

#### Why does my resume not appear on my GitHub homepage?

- case 1: You have named your markdown file incorrectly

To correct this, rename your resume file to index.md.

- case 2: You have placed your resume in the wrong directory

To correct this, move your file from the folder it sits in to the main directory of your repository.

- case 3: You have done both of the above cases

in this case, simple make the changes suggested in the previous to two cases.