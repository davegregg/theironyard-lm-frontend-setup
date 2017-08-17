# Git

* `brew install git`
* Open a fresh Terminal tab and check the version.
	* `git --version`
	* Should read `git version 2.11.0` (or higher)
    * If it doesn't, try `brew upgrade git`
* Remember when you set up an account on [GitHub](https://www.github.com) (it was in the prework). Well, we need to tell Git who you are there so things will match up later.
	* `git config --global user.name "YOUR NAME"`
	* `git config --global user.email "YOUR EMAIL ADDRESS"` (this should be the same email address you used to sign up for GitHub)
	* `git config --global credential.helper osxkeychain` (rather than go into detail on what this does, [see GitHub's docs](https://help.github.com/articles/caching-your-github-password-in-git/).
    * If you're feeling more adventurous, go with the SSH key approach
      outlined here: <https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/>
* We're going to want to ignore some Mac-specific files in our git commits. Run the follow commands:
  * `echo .DS_Store >> ~/.gitignore_global`
  * `git config --global core.excludesfile ~/.gitignore_global`

## Caveat

There is only a single application we're going to ask you to _not install_ during class:

[GitHub for Mac](https://mac.github.com), which is the non-commandline (GUI) version of `git`.

It's a fine app, but for class purposes, we want to learn Git from the bare metal. That way, the GitHub desktop app will actually make sense if you decide to use it later in your career.
