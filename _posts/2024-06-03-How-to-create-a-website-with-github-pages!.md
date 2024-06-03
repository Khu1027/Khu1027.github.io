---
layout: post
title: How to create a website with github pages
subtitle: The quick and easy way to create a website for free!
thumbnail-img: /assets/blog-img/gitpagestut/github-pages-examples.png
gh-repo: Khu1027/Khu1027.github.io
gh-badge: [star, fork, follow]
tags: [ghpages]
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
1. Create a GitHub Pages Repository
2. Add a simple Jekyll theme

## 1. Create a bare-bones website

> 1) Create a GitHub Account
This can be done by going to [Github.com](https://github.com/) and signing up to a new account

> 2) Create a new repository

{: .box-error}
Your repository **MUST** be named **[YOUR_GITHUB_USERNAME].github.io**. Other names will not work correctly

Once you have an account, make a new repository with the following details <br/>
- Ensure your repository is named **[YOUR_GITHUB_USERNAME].github.io**
    - For example my username is Khu1027, so my respository would be _Khu1027.github.io_
- Make sure your repository is public
- You can select the option to add a README.md when creating your repo

Create your repo and commit any changes

![Create a Repository](/assets/blog-img/gitpagestut/git_new_pages.png)

> 3) Add a **index.html** file to your repository

{: .box-note}
You can add a new file directly on your github repository <br/>
For more advanced users, you can clone the repository to your own computer and use this to add files, and commit and push changes

- Create an **index.html** file (or **index.md** file if you want to use markdown)
- Add any text/base website code that you have (this file is the first page that will be shown on your website)
- You can go back and edit/change this page to your liking at any time!
- Commit your changes

![Create Index.md file](/assets/blog-img/gitpagestut/create_index_file.png)

> 4) Edit your Repo Settings for GitHub Pages

- Click on **Settings** on the navbar at the top of your repo
- Click on **Pages** on your settings sidebar
- On _Build and deployment_ select *Deploy from a branch*
- From _branch_ select **main** and then **/(root)** and save

![Edit Repository Settings](/assets/blog-img/gitpagestut/git_pages_settings.png)