git-hub(1)
=======================================

## SYNOPSIS

`git hub [--force-origin] <contributors | issues | pull-request | stargazers | wiki>`

## DESCRIPTION

  `git(1)` extension to control your github.com (or enterprise) repo from the command-line. Works with github.com or github enterprise repos.

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

## AUTHOR

Written by Wil Moore III &lt;<wil.moore@wilmoore.com>&gt;

## REPORTING BUGS

&lt;<https://github.com/wilmoore/git-hub/issues>&gt;

## SEE ALSO

&lt;<https://github.com/wilmoore/git-hub>&gt;
