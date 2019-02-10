---
layout: post
title: 'Unix Basics: Searching for a command you previously entered'
date: 2019-02-10 00:00:00 +0000
tags:
  unix
---

Once you've been using a unix shell for a while, you'll realize that you don't have to always retype commands you've run before. You can use the "up" key on your keyboard to look for commands you typed previously.

After a while, this too gets a bit tedious. So from time to time it's useful to type

	history

This will show a list of commands you have run on the terminal. If you are lucky enough you'll find your command there and you can just type it again or push the "up" key until you find it.

When trying to get the exact command (say it has some configuration details or and address) I've seen some people do the following to find the command:

	history | grep ssh

And this is fine. However, some of this people would benefit from using reverse search on the terminal. You can access this by pressing Control and the 'r' key and typing the command you are looking for

If the search result wasn't the one you wanted, just keep pressing Control + r and it will give you the next result!

If you want to execute a result just press the Return key or you can start editing directly.

<!--
(See also: [`kebab-case`](https://en.wikipedia.org/wiki/Letter_case#Special_case_styles),
[`SCREAMING_SNAKE_CASE`](https://github.com/rubocop-hq/rubocop/blob/4a0d6361d0065ca16ba19bdf3b3d6c4623e14adc/lib/rubocop/cop/naming/constant_name.rb#L7).)
-->
