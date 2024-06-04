---
layout: post
title: How to create a website with GitHub Pages
subtitle: The quick and easy way to create a website for free!
thumbnail-img: /assets/blog-img/gitpagestut/github-pages-examples.png
gh-repo: Khu1027/Khu1027.github.io
gh-badge: [star, fork, follow]
tags: [github-pages]
author: Khulood Ahmad
---

{: .box-success}
**Welcome to my new coding blog!** <br/>
As the first blog post I thought it was only appropriate to explain step-by-step how I made my own website/blog and hosted it using GitHub's free hosting service, GitHub Pages, for free!

<!-- ![GitHub Pages Logo](/assets/blog-img/gitpagestut/github-pages-examples.png) -->
<div style="text-align: center;">
    <img src="/assets/blog-img/gitpagestut/github-pages-examples.png" alt="GitHub Pages Logo" width="200"/>
</div>

## What is GitHub Pages?

[GitHub Pages](https://pages.github.com/) is a free hosting service that allows GitHub users to create and host their own unique website for free! Files are taken straight from your repository on GitHub and deployed automatically whenever you push to the repo

## Why should you use GitHub Pages? (compared to other hosting platforms)

- **First of all, its _FREE_** <br/>
    Any person familiar to hosting applications and websites should know what a nightmare it is to host their site online cheaply or for free. 
- **Secondly, its _EASY_** <br/>
    It is not an exaggeration to say that you can make a basic website on GitHub pages in _minutes_. The ease of use is incredible. _But_ you may experience some hiccups when you first get started, so I'm here to make it just a bit easier for you :)
- **Last but not least, it is connected directly to your GitHub account** <br/>
    Programmers and coding enthusiasts would be glad to know that everything is integrated to your GitHub account. Your website is automatically updated whenever you push to your repository :D
- **And many other features I have yet to discover!**

# The step-by-step guide to making your own website

There are multiple ways in which you can start your own GitHub Pages site.
However for this blog I will be going through the bare basics on how to 
1. Create a bare-bones website
2. Add a simple Jekyll theme

{: .box-warning}
**Some things to note** <br/>
If you will be editing your website on a local computer code editor such as vscode, you might want to download all the necessary libraries and plugins, to your computer, to avoid any issues when using themes and other GitHub Pages extensions.<br/>
These include: Ruby, Bundler, Jekyll, GitHub Pages Gem

## 1. Create a bare-bones website

<h3> 1) Create a GitHub Account </h3>
This can be done by going to [Github.com](https://github.com/) and signing up to a new account

<h3> 2) Create a new repository </h3>

{: .box-error}
Your repository **MUST** be named **[YOUR_GITHUB_USERNAME].github.io**. Other names will not work correctly

Once you have an account, make a new repository with the following details <br/>
- Ensure your repository is named **[YOUR_GITHUB_USERNAME].github.io**
    - For example my username is Khu1027, so my respository would be _Khu1027.github.io_
- Make sure your repository is public
- You can select the option to add a README.md when creating your repo

Create your repo and commit any changes

![Create a Repository](/assets/blog-img/gitpagestut/git_new_pages.png)

<h3> 3) Add a index.html file to your repository </h3>

{: .box-note}
You can add a new file directly on your github repository <br/>
For more advanced users, you can clone the repository to your own computer and use this to add files, and commit and push changes

- Create an **index.html** file (or **index.md** file if you want to use markdown)
- Add any text/base website code that you have (this file is the first page that will be shown on your website)
- You can go back and edit/change this page to your liking at any time!
- Commit your changes

![Create Index.md file](/assets/blog-img/gitpagestut/create_index_file.png)

<h3> 4) Edit your Repo Settings for GitHub Pages </h3>

- Click on **Settings** on the navbar at the top of your repo
- Click on **Pages** on your settings sidebar
- On _Build and deployment_ select **Deploy from a branch**I
- From _branch_ select **main** and then **/(root)** and save

![Edit Repository Settings](/assets/blog-img/gitpagestut/git_pages_settings.png)

<h3> 5) Congrats! You've made your website! </h3>

- You can check your website by going on your repo settings and Pages
- You should see a new area at the top of the page that says _Your site is live at..._
- Click on the link to see your site!
- Your website will automatically deploy whenever you push to your repo

![GitHub pages live](/assets/blog-img/gitpagestut/git_page_live.png)

## 2. Add a Jekyll theme

{: .box-note}
**What is a Jekyll theme?**<br/>
[Jekyll](https://jekyllrb.com/docs/themes/) is an _'extensive theme system'_ that you add to your GitHub Pages website to get a desired theme/look to your site

<h3>1) Choose a theme for your website</h3>

Jekyll has a vast array of themes which you can choose from. These include [Themes supported by GitHub Pages](https://pages.github.com/themes/) which are very simple to add.

Or themes created by individuals that can be found on [Jekyllthemes.io](https://jekyllthemes.io/). My website is created using the [Beautiful Jekyll](https://github.com/daattali/beautiful-jekyll#readme) theme by Daattali on GitHub. 

For this tutorial, I will be demonstrating how to add the themes supported by GitHub Pages. 

<h3>2) Follow the repo instructions to add the theme</h3>

For this tutorial I will be using the [Architect Theme](https://github.com/pages-themes/architect) which looks like [this](https://pages-themes.github.io/architect/)

Most (if not all) GitHub Pages Themes have easy-to-follow instructions to add the theme in the repository's _README_

<h3>3) Create the necessary files to add the theme</h3>

Jekyll themes make use of the _config.yml configuration file to add the theme to the GitHub Pages.<br/>
If the theme requires you to add lines to your _config.yml file, and you do *not* have the file in your repository, simply create a new file of type _config.yml and add the code.

A **Gemfile** is another file you can add to your root repository, with settings to describe the gem dependencies required to run a Ruby program. In the case for the Architect Theme, the GemFile is used to change how you preview your site on your computer

#### Architect theme requires the following code in the _config.yml file

{% highlight yaml linenos %}
remote_theme: pages-themes/architect@v0.2.0
plugins:
- jekyll-remote-theme # add this line to the plugins list if you already have one
{% endhighlight %}

#### Architect theme requires the following code in the GemFile file

{% highlight text linenos %}
gem "github-pages", group: :jekyll_plugins
{% endhighlight %}

![Architect Repo](/assets/blog-img/gitpagestut/Architect-repo.png)

<h3>4) Voila! Your Site is beautified</h3>

Once you have saved/commit/pushed your changes, you're essentially done!!<br/>
Wait until GitHub has automatically deployed your website again to see your changes


## Congrats! You just made and hosted your first website!

I will link some resources that really helped me when creating my own blog. **Remember!** this is a _barebones_ website, but a canvas of infinite possibility. </br>
 I may make another blog on how I used the [Beautiful Jekyll](https://github.com/daattali/beautiful-jekyll?tab=readme-ov-file#add-your-own-content) theme and tailored it to my liking as that was a different process.

Essentially, if you want to use an existing website template, **Check the repository first before making your own!** Some templates may require you to _fork_ from an existing repository or download files (meaning you will need to delete any files/your whole github.io repository)

Thank you for reading! More interesting blog posts to come I promise!

## Resources

[A full in-depth tutorial (much more detailed than mine TT) on GitHub Pages](https://tomcam.github.io/least-github-pages/)

[Official GitHub tutorial on adding a Jekyll theme](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll)

[GitHub Pages Supported Themes](https://pages.github.com/themes/)

[Jekyll Themes](https://jekyllthemes.io/)

[Beautiful Jekyll Repository](https://github.com/daattali/beautiful-jekyll?tab=readme-ov-file#add-your-own-content)

[Basic Markdown Syntax](https://www.markdownguide.org/basic-syntax/)