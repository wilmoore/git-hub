git-hub(1)
=======================================

## SYNOPSIS

  `git hub [--force-origin] <contributors | issues | pull-request | stargazers | wiki>`

## DESCRIPTION

  Extension to control your Github repo from the command-line.
  Works with public Github.com or github:enterprise repos.

## RATIONALE

  I love git and Github. I love the shell/terminal. After doing
  ["focussed"][git-process] work in a topic branch, I want to type
  `git hub pull-request` or `git hub issues` or `git hub` and be
  taken to the expected location on the Github website.

  This extension does not require Ruby and does not require you to
  provide username, password, or API key.

## COMMANDS

  Omit the command (i.e. just type `git hub`) and you'll be taken
  directly to the main github page of your repo.


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
    % git clone https://github.com/wilmoore/git-hub.git
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

## INSPIRATION

- [hub](https://github.com/defunkt/hub)
- [git-extras](https://github.com/visionmedia/git-extras)

## AUTHOR

Written by Wil Moore III &lt;<wil.moore@wilmoore.com>&gt;

## REPORTING BUGS

https://github.com/wilmoore/git-hub/issues

## LICENSE

    (The MIT License)

    Copyright (c) 2012 Wil Moore III <wil.moore@wilmoore.com>

    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is furnished
    to do so, subject to the following conditions:
    
    The above copyright notice and this permission notice shall be included in all
    copies or substantial portions of the Software.
    
    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.


[git-process]:  https://github.com/jdigger/git-process
