vim-bracketed-paste enables transparent pasting into vim. (i.e. no more `set paste`!)

Installation
============

I recommend using [pathogen](https://github.com/tpope/pathogen). Once you have installed pathogen:

```bash
cd ~/.vim/bundle
git clone https://github.com/ConradIrwin/vim-bracketed-paste
```

Otherwise just copy-paste everything from [plugin/bracketed-paste.vim](https://github.com/ConradIrwin/vim-bracketed-paste/blob/master/plugin/bracketed-paste.vim) into your `~/.vimrc`.

Usage
=====

You need to be using a modern xterm-compatible terminal emulator (xterm, urxvt, and iTerm2 are known to work, and modern gnome-terminal should too) that supports [bracketed paste mode](http://cirw.in/blog/bracketed-paste).

Then whenever you paste into your terminal emulator using `command+v` or `shift+insert`, vim will automatically `:set paste` for you.

Credit
======

The code for this plugin was taken from Chis Page's answer to a [StackOverflow question](http://stackoverflow.com/questions/5585129/pasting-code-into-terminal-window-into-vim-on-mac-os-x), I just packaged it.
