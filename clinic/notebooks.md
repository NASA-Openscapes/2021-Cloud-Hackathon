---
title: Notebooks, Python, GitHub
---

## Summary

In this session, we will provide a brief introduction to:

1.  Command line (**terminal**/shell)
2.  Version Control (code management using **git**)
3.  Programming in **Python** (using Jupyter Notebook)
4.  Geospatial Fundamentals (optional, self-study)

You will need a working knowledge of git and terminal for this hackathon. We will provide an overview of these topics and also share resources for self-paced learning.

## Introduction :: Command Line (Terminal/Shell)

#### Shell Basics

1.  [What is Terminal or Shell?](https://swcarpentry.github.io/shell-novice/01-intro/index.html)
2.  [Navigating Files and Directories](https://swcarpentry.github.io/shell-novice/02-filedir/index.html)
3.  [Working with Files and Directories](https://swcarpentry.github.io/shell-novice/03-create/index.html)

#### Shell: More Details

Detailed self-paced lesson on shell: [Shell Lesson from Software Carpentry](http://swcarpentry.github.io/shell-novice/)

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

#### Git Commands: Summary

| Git Command  | Summary                                                                                                                         |
|--------------|---------------------------------------------------------------------------------------------------------------------------------|
| `git status` | Shows the current state of the repository: the current working branch, files in the staging area, *etc.*                        |
| `git add`    | Adds a new, previously untracked file to version control and marks already tracked files to be committed with the next `commit` |
| `git commit` | Saves the current state of the repository and creates an entry in the log                                                       |
| `git log`    | Shows the history for the repository                                                                                            |
| `git diff`   | Shows content differences between commits, branches, individual files and more                                                  |
| `git clone`  | Copies a repository to your local environment, including all the history                                                        |
| `git pull`   | Gets the latest changes of a previously cloned repository                                                                       |
| `git push`   | Pushes your local changes to the remote repository, sharing them with others                                                    |

: Commonly used git commands (modified from [source](https://uwhackweek.github.io/jupyterbook-template/tutorials/jupyter.html))

#### Git: More Details

**Lesson**: For a more detailed self-paced lesson on git, visit [Git Lesson from Software Carpentry](http://swcarpentry.github.io/git-novice/)

**Cheatsheet**: [Frequently used git commands](https://training.github.com/downloads/github-git-cheat-sheet.pdf)

**Dangit, Git!?!**: If you are stuck after a git mishap, there are ready-made solutions to common problems at [Dangit, Git!?!](https://dangitgit.com/en)

## Introduction :: Programming in Python

Switch to Jupyter Notebook for an introduction to programming in Python

-   Variables (and mathematical operations)
-   [Data Structures](https://swcarpentry.github.io/python-novice-inflammation/04-lists/index.html) (list, tuple, dict)
-   [Flow Control](https://swcarpentry.github.io/python-novice-inflammation/05-loop/index.html) using loops (for, while)
-   [Conditionals](https://swcarpentry.github.io/python-novice-inflammation/07-cond/index.html) (if, else, elif)
-   [Functions](https://swcarpentry.github.io/python-novice-inflammation/08-func/index.html)
-   [Errors and Exceptions](https://swcarpentry.github.io/python-novice-inflammation/09-errors/index.html) (understanding and handling errors)
-   Using modules (libraries, packages)
    -   [pandas](https://pandas.pydata.org/docs/): high-performance, easy-to-use data structures and data analysis tools
    -   [rioxarray](https://corteva.github.io/rioxarray/stable/): based on the rasterio package for working with rasters and [`xarray`](http://xarray.pydata.org/en/stable/)

#### Python Learning Resources

Self-paced lesson on [Programming with Python](https://swcarpentry.github.io/python-novice-inflammation/) from Software Carpentry

## Introduction :: Geospatial Fundamentals (Optional)

Detailed self-paced lesson on [Fundamentals of Geospatial Raster and Vector Data with Python](https://carpentries-incubator.github.io/geospatial-python/) from Data Carpentry
