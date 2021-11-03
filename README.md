# Hosting a Static Site on GitHub Pages

The purpose of this README is to show you how to upload a resume formatted in markdown onto GitHub pages using a static site generator. The resulting site will have a few features, the prominant one being that we won't need to write any XML or HTML/CSS, the other features are easy to change themes and a fully responsive site. A responsive site is a site that changes it's features to maintain a good visual appearance on multiple screen sizes.

## Some Prerequities

Before we get started, you will need to set a few things up. You will need the following:

- A GitHub account

GitHub is a distributed version control system, and it will be needed to host your GitHub pages site.

- A resume formatted in markdown

If you are not already familiar with markdown, refer to the _More Resources_ section where I have linked a markdown tutorial, as well as a markdown cheet sheet to help you make your markdown formatted resume.

- A markdown editor

You will use the markdown editor to create your resume and any other content on your GitHub pages site. I used Byword, it is very minimal, has a preview for your formatted text, and has great text highlighting.

- (Optional) Jekyll

This is optional, but will speed up the development of your site by reducing the number of commits you need to make, and in turn, reduce the time you spend waiting for GitHub to show the changes you make to your site. There is a link in the _More Resoures_ section that shows you how to install Jekyll.

## Instructions

1. Set up our GitHub Pages repository:

	- Sign in to Github. 
	- Click the "+" button in the top right hand corner of the screen
	- Click on "New repository".
	- Type (your_user_name).github.io in the repository name field, your_user_name needs to match the user name to the left of the "/" verbatim
	- Leave all other settings as their default values.
	- Press the "create repository" button.

A Github repository is a form of a distributed version control system or DVCS for short, as mensioned by Etter in his book Modern Technical Writing;
> DVCS have better performance, allow for offline work, and are superior for concurrent work on the same file.
Though not completely relavent to this task, knowing the many features of DVCS help when working on projects in a group, as well as aid in building your site more effectively.

2. Set a theme for your GitHub pages site:

	- Click the Settings button towards the right of the top bar.
	- Click the pages tab towards the bottom of the navigation bar on the left.
	- Click the change theme button.
	- Select a theme from the top bar.
	- Click the green select theme button.

I opted to use the slate theme as it is simple and does not drag your focus away from the main content.

Etter mentions in his book,
> you provide a static site generator with content (lightweight markup) and a theme (templated HTML and CSS), and it processes everything into a working website.
In other words, Jekyll takes as input the theme and markdown, and outputs a site built with HTML and CSS.

	- Go to the code tab towards the left top bar, after selecting a theme.

3. Uploading resume to GitHub

	- Ensure your resume file is named _index.md_

As mentioned in the previous step, this file will be the markdown input to Jekyll.

	- Return to GitHub
	- Open the add file drop down
	- Click upload files
	- Drag and drop index.md into the designated area
	- Add a title for the commit,
	- Optionally, add some comments
	- Press commit changes.

Commits are what allow many individuals to contribute to a project, these commits need an internet connection, thus any progress can be stored locally until internet is present, where the commit can take place. This is directly related to how DVCS work as menstioned in part 1.

It can take time for the changes you make to become visible on your GitHub pages site, this delay is caused by GitHub. The best way to bypass this wait interval is to develop your site locally with Jekyll until the results are satisfactory, and then commit the final result. When testing locally, Jekyll will make a local web server to host your site, as Etter mensions,
> You can test static websites on your local computer without installing anything and compress and ship them with software applications.
Simply put, there is no need to build a custom web server, or download a heavy web server to test your site. The primary benefits of doing is a lower storage usage and close to live updates on your site for each change you make.

4. View your now completed site

	- Search up your_user_name.github.io in your web browser, this is the home page of your GitHub pages repository, here is where you will find your resume. 

If you would like a reference, take a look at the _More Resources_ section where I have linked my own GitHub pages site, on the site I have my resume uplaoded. 

The result of following the above steps is a site containing your resume. Below is a Gif of my resume that I have hosted on my GitHub pages.

![Gif of my resume](https://github.com/diddy5436/diddy5436.github.io/blob/main/Animation.gif)

## More Resources

A few resources on markdown:

- [Learn Markdown](https://www.markdowntutorial.com)
- [A Markdown Cheat Sheet](https://www.markdownguide.org/basic-syntax/)
- A [website](https://www.oberlo.ca/blog/markdown-editors) that has a list of great markdown editors.

- my [resume](https://diddy5436.github.io) for reference.

- A link to [Etter's book](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS), it is a great resource to learn about markdown as well as useful information on technical writing.

## Authors and Acknowledgements

The contents of this repository were writen by myself with the help of the following individuals:

- Zhijie Zheng
- Akshay Sharma
- Farhan Rahman
- Kien Mai

The template I based this README off of was made by Purple Booth and can be found [here](https://github.com/PurpleBooth/a-good-readme-template).

## FAQ

**Q: Why is Markdown better than a word processor?**

**A:** Word processor's main funtion is to create PDFs, however, in many cases, we don't want to simply download our information as a PDF, we want something that can continue to change, and also have a variety of ways to represent the information. With markdown, we can represent our information in simple text, slide shows, and websites. There are many more ways of presenting markdown, which makes it far superior to a word processor in many areas.

**Q: Why does my resume not appear on my GitHub homepage?**

**A:** There are three main causes for this issue, they are as follows:
 
- case 1: You have named your markdown file incorrectly

To correct this, rename your resume file to index.md.

- case 2: You have placed your resume in the wrong directory

To correct this, move your file from the folder it sits in to the main directory of your repository.

- case 3: You have done both of the above cases

in this case, simple make the changes suggested in the previous to two cases.