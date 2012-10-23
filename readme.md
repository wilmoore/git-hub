git-hub(1)
=======================================

## SYNOPSIS

`git hub [--force-origin] <contributors | issues | pull-request | stargazers | wiki>`

## DESCRIPTION

  extension to control your github.com (or enterprise) repo from the command-line. Works with github.com or github enterprise repos.

## RATIONALE

  ...

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

## INSTALLATION

  % mkdir ~/local
  % cd !$
  % git clone git://github.com/wilmoore/git-hub.git
  % cd git-hub

  # ~/.bash_profile
  export PATH=$HOME/local/git-hub/bin:$PATH
  source $HOME/local/git-hub/etc/bash_completion.sh

  # update to latest
  % cd $HOME/local/git-hub
  % git pull origin master

  # update to a tag
  % cd $HOME/local/git-hub
  % git checkout x.x.x

## AUTHOR

Written by Wil Moore III &lt;<wil.moore@wilmoore.com>&gt;

## REPORTING BUGS

&lt;<https://github.com/wilmoore/git-hub/issues>&gt;

## SEE ALSO

&lt;<https://github.com/wilmoore/git-hub>&gt;
