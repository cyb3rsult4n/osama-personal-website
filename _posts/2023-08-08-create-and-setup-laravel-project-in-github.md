---
title: Create and Setup Laravel Project in Github
tags:
- ''
- development
- backend
- laravel
- github
- git
post-image: https://raw.githubusercontent.com/omar-danasoury/personal-website/master/assets/images/posts/laravel.jpg
---

In this blog, we will be discovering how to start and setup a laravel project in Github to start our development using Laravel!

First, create a blank repo in github with no readme.md.

Hold on, do not clone it now, instead, create a laravel project at your preferred folder (for me I will use htdocs) using the following command.  

But before getting into the commands, note that `your-project-name` should be identical to the name of the repo we have made before.

Let's get back and create our Laravel project using the following command:

``` bash
composer create-project laravel/laravel your-project-name
```

or use this command if you want to utilize Laravel's installer:

``` bash
laravel new your-project-name
```

Then after the project is made, initialize a repo by running:

``` bash
git init
```

Then add all files and commit them

``` bash
git add .
git commit
```

The following step is optional, which is renaming the branch from master to main. if you wanna do this, run:

``` bash
git branch -M main
```

After that, all we need is to set the `origin` remote repository link we can push to our remote server in Github later.
if you run `git remote -v` you will get empty result at this point as we did not add anything yet.  

Note that the name `origin` can be changed to any name you prefer. I prefered to use it to represent our remote repository hosted on github.

So let's run the following command:

``` bash
git remote add origin your-remote-repo-link
```

Finally, we will set the upstream to the same remote repo so we can push to the remote repository on Github.

``` bash
git push -u origin main
```

And  congratulations, you can now work on your laravel project and use git and github to do version control for your project.  

If you found this useful, feel free to share it with your friends and colleagues to help them out.  

Enjoy, and have a nice day!
