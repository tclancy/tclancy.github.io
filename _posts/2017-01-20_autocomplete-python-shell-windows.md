---
layout: post
title: Autocomplete in Python Shell on Windows
tags: [python,windows,frustration]
author: Tom Clancy
---

# Autocomplete in Python Shell on Windows

Because I drive myself insane replicating this when I find I want autocomplete on Windows, here are the steps (as of January 2017 anyway):

* `pip install pyreadline`
* `pip install ipython[shell]`

Except right now step 2 fails when installing `scandir` so I grabbed it [here](http://www.lfd.uci.edu/~gohlke/pythonlibs/#scandir), installed the .whl file via pip and then ran that second step.
