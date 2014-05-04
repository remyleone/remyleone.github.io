---
layout: article
title: ssh trick for heavy github user
tags:
  - code
  - productivity
---

If like me you use github, bitbucket and more generally git a lot, here
is a trick you might be interested in.

A typical git clone command look like this:

    git clone git@github.com:sieben/dotfiles.git

Even if this is very straightforward, there is something simpler that
can be done. Just open your .ssh/config and add the following lines:

    Host github
    HostName github.com
    User git

Congratulations! Now, you can type:

    git clone github:sieben/dotfiles.git

Of course, you can adapt this trick to bitbucket and your own git
servers.
