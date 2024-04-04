Module 23: Communicating Results with Data
Required GitHub activity: Publishing an interactive site or dashboard

Using GitHub to host websites
Your GitHub repositories are not only useful for storing, updating and collaborating on code files; they can also be used to host static websites. This means that basic HTML documents can be delivered using a URL provided by your GitHub repository. In this activity, you will explore two approaches to building websites in GitHub by either creating HTML documents directly or using an existing template site with Jekyll.

Creating a new repository
To begin, you will use HTML files directly to create a website using GitHub Pages. First, create an empty repository.


Now, create a new file called index.html with the ‘create new file’ link in your new repository.

Edit the index.html file and add some basic HTML, such as:


Commit your changes and go to the settings using the ‘Settings’ tab from your repository. Here, select the Pages link from the left sidebar.

Now, you can select what the root of your website will be. In this example, you simply need to specify the main branch of your repository that contains the HTML page.


Save these changes and wait a minute before refreshing your page. After taking root, this should generate a URL to the page username.github.io/html_site/, similar to the following:

Following the link, you should find a page with the HTML file rendered as follows:

While this site would still need some work for a portfolio, the idea is that once you have the HTML files together, they are easily shared using GitHub Pages. Many templates exist for basic portfolio sites. If you are comfortable with static files, such as HTML and CSS, this is a straightforward approach to building and displaying a website.

Creating a portfolio site with Jekyll
While HTML file displaying is straightforward, unless you have a background in styling the pages, it may be overly cumbersome to get a good-looking site. Instead, there are libraries that contain more preset elements that can produce static web pages, including Jekyll, which integrates easily with GitHub. In the example below, you will clone an existing template site and update the code to represent a simple portfolio site that is also hosted through Pages.

Forking a template
Rather than installing anything locally (using Jekyll locally requires Ruby, which can be difficult to install), you will fork a template repository that can be adjusted and updated with your own information. There are many examples of such repositories. Here, you will use LeNPaul's portfolio-jekyll-theme repository located here.
The first step is to create a fork of the repository using the ‘Fork’ button in the upper-right corner of the repositories home page as follows:


This will create a copy of the repository in your GitHub. This is a Jekyll site that has already been set up, so you just need to alter a few things to link it with GitHub Pages. From here, in the ‘Pages’ tab of the settings for the repository, deploy the repository from the gh-pages branch as follows:

After this, the site should be live and linked through the URL https://username.github.io/portfolio-jekyll-theme and show something like the following:

The pages themselves are just markdown files and can be edited in the pages folder. For example, you can update the about.md file and commit your changes.

Returning to the about page, you would now see the following:

The social links can be updated in the _data/config.yml file. Again, this is just one available theme; however, it is easy to implement and update and provides most of the basic functionality you would want from a portfolio site. Consider trying different themes and identifying one that you prefer using for your portfolio.





Combining with Jupyter Notebooks
Another advantage of Jekyll is that you can easily convert projects in Jupyter Notebooks to markdown files and add them as pages in the site. For example, this notebook can be converted using the built-in nbconvert functions of Jupyter as follows:
jupyter nbconvert --to markdown github_pages.ipynb
Then, this markdown version can be uploaded to your repository as a blog post in the _posts directory. From here, you can simply add the required metadata and change the filename to abide by the convention YYYY-MM-DD and the meta information required for the pages added to the top as follows:
---
layout: post
title: "Using github pages"
—

After committing the changes, the page will be visible at username.github.io/portfolio-jekyll-theme/github-pages:

Most Jekyll themes will work in a similar way, and the markdown files are easily created from Jupyter Notebooks. You are encouraged to adjust the example or another template that you find to begin a basic portfolio site for yourself.

Activity submission
To complete this activity, submit the link to your newly created static website in Canvas. On the front page, your website should include an ‘About you’ section. In this section, share a little about yourself, such as your name, location, education, industry, recent projects, goals and professional or personal interests.








Professional Certificate in Data Analytics	                                                        	 Page 1 of 2


