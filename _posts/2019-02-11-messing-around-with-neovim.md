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
https://linode.com/docs/tools-reference/tools/how-to-install-neovim-and-plugins-with-vim-plug/
-->

The first thing I like doing on new neovim instances is changing the colorscheme to something nicer like desert 
or elflord:

	:colorscheme desert

I think one of the coolest things about neovim is being able to run a terminal WITHIN a vim window. You do this by running:

	:terminal

Or simply:

	:te

Pressing the A key will "append" as in normal mode in regular vim and you should be able to use your terminal as 
usual. Pressing: <C-\> <C-n> (control+\ followed by control+n) will let you access "vim mode" over the terminal.

If you are on Windows, the terminal will open a command prompt terminal. But I really recommend using PowerShell instead.
This is very simple to set up by running the following command in Normal mode:

	:set shell=powershell

That's the basics! If you want to set up a configuration file do look forward to my next post on neovim's init.vim config file. Till we meet again!
	
<!--
There are more options below or in my .vimrc file. Let's come back to this
https://stackoverflow.com/questions/36108950/setting-up-powershell-as-vims-shell-command-does-not-seem-to-be-passed-correct
-->
