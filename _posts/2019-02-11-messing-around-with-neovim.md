---
layout: post
title: 'Messing Around with Neovim'
date: 2019-02-11 00:00:00 +0000
tags:
  vim
  unix
  sys-admin
---

First of all let's install neovim. If you are on Ubuntu or Debian, the following should work:

	sudo apt install nvim

I think brew works on Mac but I haven't tested it. On Windows, you can download a release from github and
extract it somewhere you consider appropriate

Let's also install the neovim python module (a variation of the following command should work):

	pip3 install --user neovim

Let's do a quick test:

	python -c "import neovim"

OK! So now that we have NeoVim installed let's open the qt-gui application or run it in the command line using:

	nvim

<!-- To install plugins
https://github.com/junegunn/vim-plug
-->

The first thing I like doing on new neovim instances is changing the colorscheme to something nicer like desert 
or elflord:

	:colorscheme desert

I think one of the coolest things about neovim is being able to run a terminal WITHIN a vim window. You do this by running:

	:terminal

Pressing the A key will "append" as in normal mode in regular vim and you should be able to use your terminal as 
usual. Pressing: <C-\> <C-n> (control+\ followed by control+n) will let you access "vim mode" over the terminal.
