---
title: Notebooks, Python, GitHub
---

## Summary

In this session, we will provide a brief introduction to:

1.  Using command line (**terminal**/shell)
2.  Code management (using **git**)
3.  Fundamentals of programming in **Python**

You will need a working knowledge of git and terminal for this hackathon. We will provide an overview of these topics and also share resources for self-paced learning.

## Introduction :: Command Line (Terminal/Shell)

#### Shell Basics

1.  What is Terminal or Shell?
2.  Navigating Files and Directories
3.  Working with Files and Directories

#### Shell: More Details

For a more detailed self-paced lesson on shell, visit [Shell Lesson from Software Carpentry](http://swcarpentry.github.io/shell-novice/)

## Introduction :: Version Control (Git and Github)

#### What is Version Control?

#### Configure git

Configure git with your name and email address

``` bash
git config --global user.name "Makhan Virdi"
git config --global user.email "Makhan.Virdi@gmail.com"
```

#### Store credentials

1.  Go to your github account and create a new "personal access token": <https://github.com/settings/tokens/new>

    [![Generate Personal Access Token on github.com](img/github-token.png)](https://github.com/settings/tokens/new)

2.  Configure Git to store your credentials to avoid having to enter the credentials every time.

    ``` bash
    git config --global credential.helper store
    git config -l
    ```

3.  Use a git command that requires you to enter credentials (e.g. pull, push)

    ``` bash
    git pull
    ```

4.  Provide your github "username" and "Github Token" when asked. Now your password is stored in "\~/.git-credentials" and you will not be prompted again unless the Github token expires. You can check the presence of this file using Terminal

    ``` bash
    ls -la ~
    ```

    The output looks like this:

    ``` bash
    drwxr-xr-x 13 jovyan jovyan 6144 Oct 22 17:35 .
    drwxr-xr-x  1 root   root   4096 Oct  4 16:21 ..
    -rw-------  1 jovyan jovyan 1754 Oct 29 18:30 .bash_history
    drwxr-xr-x  4 jovyan jovyan 6144 Oct 29 16:38 .config
    -rw-------  1 jovyan jovyan   66 Oct 22 17:35 .git-credentials
    -rw-r--r--  1 jovyan jovyan   84 Oct 22 17:14 .gitconfig
    drwxr-xr-x 10 jovyan jovyan 6144 Oct 21 16:19 2021-Cloud-Hackathon
    ```

    You can also verify your git configuration

    ``` bash
    (notebook) jovyan@jupyter-virdi:~$ git config -l
    ```

    The output looks like this:

    ``` bash
    user.email        = Makhan.Virdi@gmail.com
    user.name         = Makhan Virdi
    credential.helper = store
    ```

#### Clone a Repository

To clone a repository from github, copy the link for the repository and use `git clone` to create a copy of the repository:

``` bash
git clone https://github.com/NASA-Openscapes/check_github_setup
```

#### Tracking Changes

-   status
-   add
-   commit
-   log
-   diff

#### Using Remotes in GitHub

-   remote
-   pull
-   push

#### Git: More Details

**Lesson**: For a more detailed self-paced lesson on git, visit [Git Lesson from Software Carpentry](http://swcarpentry.github.io/git-novice/)

**Cheatsheet**: [Frequently used git commands](https://training.github.com/downloads/github-git-cheat-sheet.pdf)

#### Other Topics

Discuss merge conflicts and philosophy: best way to deal with merge conflicts is to avoid them; talk to your colleagues, commit often. Also can work with branches (out of the scope of this Clinic?)

## Introduction :: Programming in Python

Switch to Jupyter Notebook for an introduction to programming in Python

-   Variables (and mathematical operations)
-   Conditionals (if, else, elif)
-   Flow Control using loops (for, while)
-   Data Structures (list, tuple, dict)
-   Functions
-   Using modules (libraries, packages)
    -   pandas

## Introduction :: Geospatial Fundamentals (Optional)

Visit the detailed self-paced lesson on [Fundamentals of Geospatial Raster and Vector Data with Python](https://carpentries-incubator.github.io/geospatial-python/) on Data Carpentry website
