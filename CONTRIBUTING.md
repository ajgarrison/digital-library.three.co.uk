# Contributing to the Three Digital Library

The Three Digital Library aims to be a regularly released collaborative effort, facilitated by Team Babbage in Online. Everybody can submit problems and solutions to everyday web design issues. The Digital Library will grow with the demands of the evolving web and help us be more productive, reduce duplication of effort and make it much easier to commission work form external suppliers.

In order to help us collaborate here are the guidelines we'd like you to follow (with thanks to the Angular.js guidelines!):

 - [Getting Started](#started)
 - [Issues and Bugs](#issue)
 - [Feature Requests](#feature)
 - [Submission Guidelines](#submit)


## <a name="started"></a> Getting Started

* Make sure you have a [GitHub account](https://github.com/signup/free)

## <a name="issue"></a> Found an Issue?
If you find a bug in the source code or a mistake in the documentation, you can help us by
submitting an issue to our GitHub Repository. Even better you can submit a Pull Request
with a fix.  An example issue is available at https://github.com/ThreeUK/digital-library.three.co.uk/issues/2


## <a name="feature"></a> Want a Feature?
You can request a new feature by submitting an issue to our GitHub Repository.  If you
would like to implement a new feature then consider what kind of change it is:

* **Major Changes** that you wish to contribute to the project should be discussed first on our Digital Library Slack channel https://three-digital.slack.com/messages/digital-library-core and/or in the Mobile SOS so that we can better coordinate our efforts, prevent
duplication of work, and help you to craft the change so that it is successfully accepted into the
project.
* **Small Changes** can be crafted and submitted to the GitHub Repository as a Pull Request.

## <a name="submit"></a> Submission Guidelines

### Submitting an Issue
Before you submit your issue search the archive, maybe your question was already answered.

If your issue appears to be a bug, and hasn't been reported, open a new issue providing the following information will increase the
chances of your issue being dealt with quickly:

* Clearly describe the issue including steps to reproduce when it is a bug.
* Make sure you fill in the earliest version that you know has the issue.
* **Motivation for or Use Case** - explain why this is a bug for you
* **Browsers and Operating System** - is this a problem with all browsers or only IE8?
* **Reproduce the Error** - if you can please provide a live example or an unambiguous set of steps.
* **Related Issues** - has a similar issue been reported before?
* **Suggest a Fix** - if you can't fix the bug yourself, perhaps you can point to what might be
  causing the problem (line of code or commit)

### Submitting a Pull Request
Before you submit your pull request consider the following guidelines:

* Search [GitHub](https://github.com/ThreeUK/digital-library.three.co.uk/pulls) for an open or closed Pull Request
  that relates to your submission. You don't want to duplicate effort.
* Make your changes in a new git branch:

     ```shell
     git checkout -b my-fix-branch master
     ```
* Commit your changes using a descriptive commit message 
     ```shell
     git commit -a
     ```
  Note: the optional commit `-a` command line option will automatically "add" and "rm" edited files.

* Push your branch to GitHub:

    ```shell
    git push origin my-fix-branch
    ```

* In GitHub, send a pull request.
* If we suggest changes then:
  * Make the required updates.
  * Re-run the Angular test suite to ensure tests are still passing.
  * Rebase your branch and force push to your GitHub repository (this will update your Pull Request):

    ```shell
    git rebase master -i
    git push origin my-fix-branch -f
    ```

#### After your pull request is merged

After your pull request is merged, you can safely delete your branch and pull the changes
from the main (upstream) repository:

* Delete the remote branch on GitHub either through the GitHub web UI or your local shell as follows:

    ```shell
    git push origin --delete my-fix-branch
    ```

* Check out the master branch:

    ```shell
    git checkout master -f
    ```

* Delete the local branch:

    ```shell
    git branch -D my-fix-branch
    ```

* Update your master with the latest upstream version:

    ```shell
    git pull --ff upstream master
    ```


