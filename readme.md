git-hub(1)
=======================================

## SYNOPSIS

  `git hub [--force-origin] <contributors | issues | pull-request | stargazers | wiki>`

## DESCRIPTION

  Extension to control your Github repo from the command-line. Works with public Github.com or github:enterprise repos.

## RATIONALE

  I love git and Github. I love the shell/terminal. After doing "focussed" work in a topic branch, I want to type
  `git hub pull-request` or `git hub issues` or `git hub` and be taken to the expected location on the Github website.

## COMMANDS

  Omit the command (i.e. just type `git hub`) and you'll be taken directly to the main github page of your repo.


  `contributors`

  Visit your contributors list. Nothing wrong with a little commit vanity.

  `issues`

  Quickly navigate to the issue tracker.

  `pull-request`

  Start a new pull request from the currently active (*) branch.

  `stargazers`

  Navigate to your stargazers list.

  `wiki`

  Go to the wiki.

## OPTIONS

  `--force-origin`

  force the use of `origin` rather than `upstream`.

## EXAMPLES

    % git hub

    % git hub pull-request

    % git hub issues

    % git hub contributors

    % git hub stargazers

## INSTALL

    % mkdir ~/local
    % cd !$
    % git clone git://github.com/wilmoore/git-hub.git
    % cd git-hub

    # ~/.bash_profile
    export PATH=$HOME/local/git-hub/bin:$PATH
    source $HOME/local/git-hub/etc/bash_completion.sh

## UPGRADE

**to latest**

    % cd $HOME/local/git-hub
    % git pull origin master

**to a tag**

    % cd $HOME/local/git-hub
    % git checkout x.x.x

## UNINSTALL

Remove the following from ~/.bash_profile

    export PATH=$HOME/local/git-hub/bin:$PATH
    source $HOME/local/git-hub/etc/bash_completion.sh

Run the following command

    % rm -rf ~/local/git-hub

## AUTHOR

Written by Wil Moore III &lt;<wil.moore@wilmoore.com>&gt;

## REPORTING BUGS

&lt;<https://github.com/wilmoore/git-hub/issues>&gt;

## SEE ALSO

&lt;<https://github.com/wilmoore/git-hub>&gt;
