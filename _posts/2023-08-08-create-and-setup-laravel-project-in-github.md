---
title: Create and Setup Laravel Project in Github
tags:
- ''
- development
- backend
- laravel
- github
- git
---

In this blog, we will be discovering how to start and setup a laravel project in Github to start our development using Laravel!

First, create a blank repo in github with no readme.md.

Hold on, do not clone it now, instead, create a laravel project at your prefered folder (for me I will use htdocs) using the following command.  

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

So let's run the following command:

``` bash
git remote add origin your-remote-repo-link
```

you can add any name other than `origin` (note: redo this again and run git remote -v to see the effect of this command and to see the result that was there before running the  next command)  

Finally, we will set the upstream to the same remote repo so we can push to the remote repository on Github.

``` bash
git push -u origin main (need to understand more this command)
```

And  congratultions, you can now work on your laravel project and use git and github to do version control for your project.  

If you found this useful, feel free to share it with your friends and collegues to help them out.  

Enjoy, and have a nice day!
