# HOT Humanitarian Data Handbook

## What is this?
This repository is an experiment in using a [Git](https://en.wikipedia.org/wiki/Git) repository—for the moment on [GitHub](https://github.com)—as an open-by-default tool for the [Humanitarian OpenStreetMap Team (HOT)](https://hotosm.org) Humanitarian Data team.

It's intended to provide a single starting point for information, explanations, and resources needed to understand and manage our projects. 

__"Open by default"__ means everything here is open to _the entire world_ unless there is a specific reason to restrict access (normally personally identifiable, sensitive, or private information). It is intended to be shared and collaboratively edited by anyone in or outside of the host organization.

### Why a Git repo?
Our hypothesis is that the fork-and-pull-request workflow of Git strikes a good balance between openness (anyone can fork and/or submit a pull request) and manageability (no one has to accept pull requests, and they're very transparent and reversible).

_Why not a Wiki?_ Mostly because we think that the Git style of forking, submitting pull requests, and discussing and merging changesets handles complex information in many formats better than Wiki editing. [Here](https://about.gitlab.com/handbook/handbook-usage/#wiki-handbooks-dont-scale) is a discussion of the advantages of a Git repo over a Wiki.

_Why not folders in Google Docs?_ Mostly because it becomes tricky to know where the "official final version" of some artifact is, certainly over time and with many collaborators. Some of us find it tricky to find the Google Doc we wrote last week, let alone one written by a former colleague in 2016.

However, nothing about this specifically prohibits—or even discourages—the use of Wikis or Google Docs. As long as the Handbook contains a link to the relevant Wiki or Doc, it's perfectly all right to use either.

We've taken some inspiration from [GitLabs' handbook](https://about.gitlab.com/handbook/handbook-usage/); that company has taken a remarkably open approach to their internal workings, in part in response to some of the same challenges many of us at HOT have faced. 

## How does it work?
It's basically a Git repo full of [Markdown](https://en.wikipedia.org/wiki/Markdown) documents (like the one you're reading right now) that explain projects and processes, and contain links to relevant resources. For a reader, it's not much different from a wiki; the difference lies in how edits are proposed, merged, tracked, and managed.

Of course, a Git repo can contain almost anything. Code, images, more sophisticated text formats like [LaTeX](https://en.wikipedia.org/wiki/LaTeX), reports (as PDF of Word documents), spreadsheets, slide decks, map projects and templates, and so on (though large files like videos don't live comfortably in Git repos, it's usually preferable to keep them outside of the tracked repo and link to them). We expect that in the fullness of time the contents of the repo will become more diverse than just Markdown and links; for instance we think having easy access to a the final report on a project (not just the PDF output) will be really helpful!

A lot of documents and information will still likely live in things like Google Drive/Docs. That's fine. The Markdown documents in the handbook serve as a guide and set of links to those resources (just as a Wiki would contain links to such assets). Over time it's probably a good thing if more documents may move into the actual Git repository itself, but it's not essential that this happen.

### How can I use it?
To do more than the absolute basics, you should get some familiarity with the basics of:
- Git: cloning, committing, forking/branching, creating pull requests, and merging.
- Markdown: Creating text with styling, links, and embedded images.

[Here are some learning resources for these tools](Resources/learning_resources.md).

### Quickstart 
GitHub allows editing of text files directly from your browser. Furthermore, GitHub "speaks Markdown," so you can preview your edits to the most common kind of documentation file directly. However, we don't want people editing the "main branch" directly the way you would with a Wiki; the advantage of Git (and version control in general) is that anyone can copy, modify, and use everything in the repo, and anyone can _propose_ changes, but it's impossible for non-members to unilaterally change the ```main``` copy (and highly discouraged for members to do so; best practice is to always propose changes via a pull request and ask another member to merge them; this ensures more eyes on all changes and greatly reduces mistakes). 

If you are a member of the organization, follow the "Quickstart for members" instructions. If not, follow the "Quickstart for non-members" instructions.

#### Quickstart for members: edit a page online, then make a branch and pull request!
This is how to propose changes if you are a member of the organization, and therefore can directly edit the repository (though, again, best practice is to never unilaterally modify the ```main``` branch; always propose changes via [this workflow](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/proposing-changes-to-your-work-with-pull-requests) using [branches](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-branches) and [pull requests](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests)). 
- Click around the links available from this very page. It looks and works like a wiki to a reader, it's the editing process that is different.
- Choose a file to edit (even the one you are reading now)! Click the pencil icon at the upper right. You'll find yourself in an editing page.
- Make your changes, and preview them with the Preview Changes tab at the upper left. The [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) is a great reference for the syntax (which is quite similar to [Wiki syntax](https://en.wikipedia.org/wiki/Wiki#Editing), but GitHub—and this handbook—use Markdown, _not_ Wikitext).
- Scroll down to the bottom of the page, and select the checkbox that says "Create a new branch for this commit and start a pull request." Please _do not_ commit directly to the ```main``` branch. Make a name for your branch (something short and without spaces, for example "online-editing-instructions". 
- Click the Propose Changes button. This will create a [Pull Request](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests). 
- In the pull request window, add a description of what you've done. For small changes, a short sentence is sufficient. For large, potentially controversial changes, you should explain your reasoning thoroughly! It's also a good idea to select people to review changes, and assign someone to merge them (both reviewers and assignees can be selected on the right). Someone will (hopefully) "merge" your proposed changes when they see how helpful you have been!

#### Quickstart for non-members: fork the repo, edit a page online, and make a pull request!
GitHub allows editing of text files directly from your browser. Furthermore, GitHub "speaks Markdown," so you can preview your edits to the most common kind of documentation file directly. However, we don't want people editing the "main branch" directly the way you would with a Wiki; the advantage of Git (and version control in general) is that anyone can copy, modify, and use everything in the repo, and anyone can _propose_ changes, but it's impossible for non-members to unilaterally change the ```main``` copy (and highly discouraged for members to do so; best practice is to always propose changes via a pull request and ask another member to merge them; this ensures more eyes on all changes and greatly reduces mistakes). 

This is how to propose changes if you are _not_ a member of the organization, and therefore cannot directly modify the handbook (though it's not much different, or more difficult, than the way members propose changes). 
- Click around the links available from this very page. It looks and works like a wiki to a reader, it's the editing process that is different.
- Fork this repo. Click the Fork button, and it'll create a copy of this repository in _your_ GitHub account ([instructions here](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo#fork-an-example-repository)). 
- Now you are in your own fork (copy) of the repo. Choose any file you like (even this one that you are reading right now) and click the pencil icon at the upper right. You'll find yourself in an editing page.
- Make your changes, and preview them with the Preview Changes tab at the upper left. The [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) is a great reference for the syntax (which is quite similar to [Wiki syntax](https://en.wikipedia.org/wiki/Wiki#Editing), but GitHub—and this handbook—use Markdown, _not_ Wikitext).
- Hit the Commit Changes button at the bottom of the page. This will modify _your_ ```main``` branch, but not the original you forked from (yet).
- Create a Pull Request __TODO: add instructions__. Someone will (hopefully) "merge" your proposed changes when they see how helpful you have been!

#### Getting started by editing a page on your local computer
- Click around the links available from this very page! Again, it looks and works like a Wiki; it's the editing that is different.
- Get an account on GitHub (free to sign up).
- Fork this repo. Click the Fork button, and it'll create a copy of this repository in _your_ GitHub account ([instructions here](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo#fork-an-example-repository)). 
- Clone the repository to your local computer ([instructions here](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository)). Open it up in your file manager on your computer; you'll note that the folder structure mirrors the link structure (you can figure out where any document in the repo is by examining the URL of the link to it).
- Pick a document you want to modify.
- Make your changes to the page (Markdown document) you want to improve.
- Submit a pull request with explanation of your changes. Once it's accepted, congratulations: you are now a co-creator of the handbook.
  - Later you may be given commit privileges to the handbook, meaning you can be one of the people authorized to commit to the main branch of repo, and therefore accept (merge) pull requests (note that it's often considered a best practice to make a pull request and get someone else to merge it to main, even if you are technically able to directly commit changes to main unilaterally).

#### Getting started by creating a project
- Clone this repository. Open it up in your file manager on your computer; you'll note that the folder structure mirrors the link structure (you can figure out where any document in the repo is by examining the URL of the link to it).
- Fork the repo.
- Create a new textfile with a name like my_project.md (.md is the Markdown file extension).
- Glance at the [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) to remind yourself how to create nicely formatted text with headers, links, etc. Write an explanation of your project.
- Add a short high-level explanation of the project's main focus and goal(s). If a detailed publicly-accessible document already exists elsewhere, add a link to it.
- Try to add links to everything someone trying to manage the project would need.
  - The original project proposal and budget.
  - These may be private documents (the budget probably is). No problem; as long as the permissions _on the documents themselves_ are correctly set, the link won't help anyone who doesn't already have permission.
  - A section naming key people and their roles. For example, who is the donor/client point of contact? Who is the field team leader? Who is the HQ lead?
    - If this information should not be public, the easiest thing may be simply to put it in a Google Doc shared only with those authorized to see or edit it, and put a link to that doc in the Markdown. This way everyone will know where the document is (helpful for those who should have access to it but may not remember where it's saved; now they have a link labelled something like ```List of key stakeholders```) but only the authorized can actually read or edit it.

# Resources
## [Projects](Projects/Projects.md)

## [Learning Resources](Resources/learning_resources.md)


# Licence
[![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg
