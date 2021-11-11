---
title: Collaborative workflow
---

Here are some suggestions for collaborating with your project groups (and beyond!) using GitHub. 

This means a combination of creating a place to collaborate (a github repository) and a shared workflow to contribute. 

## Create a repository on GitHub.com

Just one person does this.

You can do this in one of your user/organization accounts, or ask someone from the Cloud Hackathon Team to create one for you in the NASA-Openscapes organization. 

Here are instructions for [creating a repo on GitHub.com](https://rstudio-conf-2020.github.io/r-for-excel/github.html#create-a-repository-on-github.com) — remember to make it public so that other hackathon folks can see and help!

## Discuss edit access vs branches

The person who created the repo will manage the permission. 

The simplest way to collaborate on GitHub is if everyone has permission to edit the repository directly through the main branch. Talk to your team — folks that have experience using branches can do so but others can push changes directly to the main branch. 

Here are instructions for [updating github repo permissions](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/managing-teams-and-people-with-access-to-your-repository#inviting-a-team-or-person). 

## Clone repo into 2i2c

Everybody does this. 

To to the JupyterHub, go to your Terminal, then: 

`git clone https://github.com/USERNAME/REPOSITORY-NAME`. 

## Check in as you push changes

Whether you're using branches or not, check in with each other as you push updates to avoid merge conflicts and have the latest progress.

Here are instructions for a [workflow with branches](https://nasa-openscapes.github.io/earthdata-cloud-cookbook/contributing/workflow.html#github-workflow) (optional).

## Uploading files from your local computer to 2i2c

*?*

## Git - Delete your local changes

There are several ways to delete your local changes if you were playing around and want to reset. Here are a few: 

**Undo changes you've maybe saved or committed, but not pushed**. This is less time and internet intensive (no new clone/download). 

If you've got changes saved, but not yet staged, committed, or pushed, you'll delete unstaged changes in the working directory with clean:

```{.bash}
cd YOUR-REPO
git clean -df
git checkout -- .
```

**Burn it all down** - delete the whole repo that you have locally, and then reclone. 

```{.bash}
cd YOUR-REPO
rm -rf YOUR-REPO
```

Here is a whole blog on how to go back in time (walk back changes), with conceptual diagrams, command line code, and screenshots from RStudio. <https://ohi-science.org/news/github-going-back-in-time>

## Git - Update local branch with remote main branch

If while you're working you would like to update your local
`your-branch` with the most recent updates on the `main` branch on
GitHub.com, there are several ways to do this. Here's one.

```{.bash}
git checkout your-branch
git fetch
git merge origin/main
```


