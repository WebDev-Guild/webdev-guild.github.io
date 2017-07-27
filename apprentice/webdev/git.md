# Git

## Intro

Git has changed the way that programmers write code forever. It provides you with a repository of all of the changes to your project over time, so you can easily go back in time to older code. You can also use Git to collaborate on the same code with other developers. Finally, services like GitHub provide extra features like Pull Requests and Issue Tracking to make large-scale collaborative projects super easy.

*It might be helpful to do the [terminal](../terminal) badge first*

## Glossary

- **Git** - A software development tool for keeping track of software versions. Can be used for code collaboration.
- **commit** - A snapshot of changes to code at a given time. Commits are identified with a unique hash of the changes. With Git, it is possible to reverse and playback changes to files to go back to older (or different) versions of a file.
- **repository** or **repo** - All of the code for your project, including all commits back to the very first commit.
- **tag** - A named commit. 
- **branch** - By going back to a previous commit, it is possible to change the code in different directions. For example, one person could branch to create a search form, while another developer creates a branch for the contact form. The code in these two branches is different.
- **HEAD** - The branch you are currently working on. 
- **master** - The default branch in a git repo. Typically the main branch showing the most stable, up-to-date code.
- **merge** - Combining the code from two branches into one branch. 
- **merge conflict** - When the code from two branches contradicts each other. For example, if you change the color of the button to be blue and I change it to be red, and then we merge the branches together, which one is correct? Hint: It doesn't become purple. Merge conflicts have to be manually resolved.
- **remote** - A git repository on another computer. It is possible to push and pull code from a remote.
- **fetch** - Getting information about the branches and tags on a remote.
- **push** - Sending a branch from your local repository to a branch on a connected remote. 
- **pull** - Fetching and merging a branch on a remote to your local repository.
- **clone** - Creating a new local repository from a remote repository. Cloning downloads the entire git history and makes it available to you locally.

There are also a number of terms specific to GitHub:

- **GitHub** - a third-party git repository hosting service.
- **fork** - creating a new remote repository on GitHub from an existing repository.
- **issue** - A comment on a git repository, typically for reporting bugs or requesting features.
- **pull request** - Making a request to the repository owner to pull from your branch or repo into the master branch.
- **release** - A special tag indicating a new version of the project.

## Suggested Learning

- Do the Git practice activity at [try.github.io](https://try.github.io/levels/1/challenges/1)
- Install Git on your computer. There are a number of guides, like [this one](https://www.atlassian.com/git/tutorials/install-git) or [this one](https://help.github.com/articles/set-up-git/).

or

- Install a client application, like [Source Tree](https://www.sourcetreeapp.com) or [GitHub Desktop](https://desktop.github.com). The application will automatically install Git for you. Client applications allow you to use git without having to use the command line interface.
- Create a free account on GitHub.

## Requirements

- Complete all of the following:
    - Create a git repository 
    - Commit some code to the repository (can be anything)
    - Create a branch on your code
    - Create a repository on GitHub
    - Connect your local repository to the remote repository on GitHub
    - Push your `master` and branch to GitHub
    - Contact your mentor to have them pass you off

## Extra Learning

- [Tutset - Git](http://www.tutset.com/fundamentals/git/) - Extra learning links
- [Git Cheat Sheet](http://www.git-tower.com/blog/git-cheat-sheet/)
- [Official Documentation](https://git-scm.com/documentation)
- [Learn Git Branching](http://learngitbranching.js.org/) - Interactive Git Branching Practice
