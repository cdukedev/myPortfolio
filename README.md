# XXX9999X - Individual Project

Git repository for ReplaceWithYourFullName

## Table of contents

1. [Instructions](#Instructions)
1. [Changes](#Changes)
1. [Issues](#Issues)

## Instructions

### Remote repository setup

Complete the following steps in the remote repository on the GitHub web site:

1. Select the `Projects` link.
1. Choose the `Create a project` button.
1. Enter a name for the project. e.g. Practice
1. Enter a description of the project.
1. Select `Automated kanban` as the template.
1. Choose the `Create project` button.
1. Three notes were automatically added in the **To do** column. Read the notes and then for each note, select the `...` in the top right corner of the note and select `Delete note`. Select `OK` to confirm deletion.

See [About project boards](https://docs.github.com/en/issues/organizing-your-work-with-project-boards/managing-project-boards/about-project-boards) for more help.

### Clone remote to local repository

In GitHub:

1. Select the `<> Code` link.
1. Select the green `Code` button.
1. Ensure **HTTPS** is selected and click the copy button to copy the remote repository URL.

In Git Bash (Windows) or Terminal (Mac, Linux)

1. Navigate to the folder where the repository should be cloned into.
1. Issue the `git clone` command followed by pasting the previously copied remote repository URL.
1. Set your user name and email using the `git config` command. E.g. `git config user.name "your name"` and `git config user.email "your email address"`.
1. Check that the correct username and email is set using the `git config -l` command.
1. Setting and checking `user.name` and `user.email` needs to be done every time the remote repository is cloned to a local repository.

Create a **develop** branch. (Only needs to be done once in a repository.)

1. Create a branch named **develop** off the main branch. E.g. `git branch develop`
1. Push the branch to the remote repository. E.g. `git push -u origin develop` Creation of files should not start until the **develop** branch has been pushed to the remote repository.
1. Switch to the **develop** branch. E.g. `git checkout develop`
1. Edit this README.md file, then at the top, replace **XXX9999X** with the course number, and replace the word **ReplaceWithYourFullName** with your full name. Save the change.
1. Stage the change. E.g. `git add README.md`
1. Commit the change. E.g. `git commit -m "Replaced name"`
1. Push the changes to the remote repository. E.g. `git push`

Merge the **develop** branch to the **main** branch.

1. Switch to the **main** branch. E.g. `git checkout main`
1. Merge the **develop** branch into the **main** branch. E.g. `git merge develop`
1. Push the changes to the remote repository. E.g. `git push`
1. Switch to the **develop** branch. E.g. `git checkout develop`

## Changes

Steps to make changes

In GitHub:

1. Assign the issue that will be worked on to yourself. See [Issues](#Issues) below.
1. If no issue exists, open a new issue and assign it to the project board and to yourself. E.g. `Create site home page` *(Ensure that the title is unique and succinct. A detailed description of what work is be completed must be entered.)
1. Double check that the issue is in the **To do** column of the assigned project board.
1. Move the issue to the **In progress** column.

In Git Bash (Windows) or Terminal (Mac, Linux):

1. Navigate to the folder where the repository was cloned into.
1. Check that the correct username and email is set using the `git config -l` command.
1. Switch to the **develop** branch and execute a `git pull` to get the latest code from the remote repository.
1. Create a new branch and switch to the new branch.
1. Add, modify and/or delete a file(s).
1. When the changes are complete:
    1. test the changes
    1. add the file(s) to the staging area
    1. commit the changes
    1. switch to the **develop** branch
    1. execute a `git pull` to get the latest code from the remote repository
    1. merge the changes to the **develop** branch from the new branch previously created
        1. resolve merge conflicts if there are any
        1. test that the code still works after the merge conflict is fixed
        1. add the file(s) fixed from the merge conflict to the staging area
        1. commit the fixed file(s)
    1. push the **develop** branch to the remote repository
    1. create a pull request on the remote repository (GitHub) from the **develop** branch to the **main** branch.
    1. review the pull request and merge to the main branch on the remote repository
1. Delete the branch previously created for coding the changes from the local and remote repositories.
1. Close the issue after all required changes have been committed. This will move the issue to the **Done** column of the project board.

Repeat these steps each time changes are to be made. **NOTE**: Ensure that a `git pull` is regularly executed while checked out on the **develop** branch to get any changes that have been pushed to the develop branch.

To keep the **develop** and **main** in sync, complete the following steps in the local repository:

1. Switch to the **main** branch. E.g. `git checkout main`
1. Pull the changes from the remote repository. E.g. `git pull`
1. Switch to the **develop** branch. E.g. `git checkout develop`
1. Merge the **main** branch into the **develop** branch. E.g. `git merge main`
1. Push the changes to the remote repository. E.g. `git push`
1. On the remote repository the develop branch will be even with the main branch.

## Issues

### Open an Issue

1. In the repository, select the `Issues` link.
1. Choose `New issue`.
1. Enter a `Title` for the issue.
1. Enter details in the `Write` tab.
1. From the **Projects** section, select the previously created project. See [Adding issues and pull requests to a project board](https://docs.github.com/en/issues/organizing-your-work-with-project-boards/tracking-work-with-project-boards/adding-issues-and-pull-requests-to-a-project-board) for more help.
1. Choose `Submit new issue`.

### Assign an Issue

1. In the repository, select the `Issues` link.
1. Select the issue that needs to be assigned.
1. Choose the `Assignees` option.
1. Select your name as the assignee to add to the issue.

### Filter issues assigned to you

1. In the repository, select the `Issues` link.
1. Choose the `Assignee` drop down.
1. Select your username from the list.

### Close an Issue

1. In the repository, select the `Issues` link.
1. Select the issue that needs to assigned to one or more group members.
1. Enter closing details in the `Write` tab.
1. Choose `Close and comment`.

### Reopen a Closed an Issue

1. In the repository, select the `Issues` link.
1. Ensure `Closed` issues are displayed.
1. Select the issue that needs to be reopened.
1. Enter reopening details in the `Write` tab.
1. Choose `Reopen issue`.

See [About issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues) for more help.
