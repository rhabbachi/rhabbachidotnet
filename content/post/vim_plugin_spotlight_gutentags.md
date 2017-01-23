+++
title = "[Vim plugin spotlight] vim-gutentags"
categories = ["vim"]
tags = ["vim","plugin", "vim-gutentags", "spotlight"]
date = "2017-01-22T17:59:20+01:00"
+++
I've recently stumbled upon this vim plugin called
[vim-gutentags](https://github.com/ludovicchabant/vim-gutentags). Historically
I've had had issue with exuberant-ctags usage via vim (or should I say,
[Universal Ctags](https://ctags.io/) usage), I remember spending quite some
time setting up the [vim-easytags](https://github.com/xolox/vim-easytags)
plugin but I didn't really managed to integrate it in my workflow. Now that I'm
thinking about it, even vim-gutentags in not really fully part of my workflow
as much as say the [tagbar](https://github.com/majutsushi/tagbar) plugin (I
really love that plugin, use it every day and makes navigating and understanding
a class or good old functions file really easy. But I digress), but I have
high hope for it but It uses the same strategy that made tagbar really work for
me: automate every step while keeping me in control. I do remember with
vim-easytags having to execute a vim command to update the tag files which was
not really what I have in mind while parsing through couple classes and
functions. Also, another problem with vim-easytags that vim-gutentags solves
very well is projects folder detection, vim-gutentags brilliantly detects the
vcs currently in-use and assumes that the project root directory. Sure this
call pull in some un-related content to be parsed into the tags file but that's
not really an issue for me.

One default setup of vim-gutentags that did not really for me is the cache tags
file placement. By default, vim-gutentags will place the tags file on the root
of the current repo. This was causing two side effects:

- This will generate noise on the git commands output like `git status` and
   `git diff`. Not workflow breaking bot kind of annoing.

- Grepping (or in my case, [silver searching ...]
(https://github.com/ggreer/the_silver_searcher)) the whole repo will pollute
the output with annoying noise. (again not a major workflow breaking,
but really really annoying to have to go back and add the file to the --ignore
option).

What I ended up doing is use the [g:gutentags_cache_dir
option](https://github.com/ludovicchabant/vim-gutentags/blob/master/doc/gutentags.txt#L385)
to put all the cache tag files into a specific directory (in my case, it the
[`~/.vimtags`
folder](https://github.com/rhabbachi/dotfiles/blob/master/home/.vimrc.bundles.local#L184)).
This what that folder looks like now:

![.vimtags folder](/images/dots_vimtags_content.png).

I'm really looking forward to finding new ways to leverage the exuberant-ctags
feature while working in vim (which is where I spend most of my time anyway).
