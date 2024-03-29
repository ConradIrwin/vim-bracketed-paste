vim-bracketed-paste enables transparent pasting into vim. (i.e. no more `:set paste!`)

Installation
============

Vim supports native package directories starting with version 8. All you have to do is clone this project under `~/.vim/pack/<any dir name>/start/vim-bracketed-paste` to have it auto-load.

```bash
mkdir -p ~/.vim/pack/dist/start
git clone https://github.com/ConradIrwin/vim-bracketed-paste ~/.vim/pack/dist/start/vim-bracketed-paste
```

For Vim 7 and older, I recommend using [pathogen](https://github.com/tpope/vim-pathogen). Once you have installed pathogen:

```bash
cd ~/.vim/bundle
git clone https://github.com/ConradIrwin/vim-bracketed-paste
```

Otherwise just copy-paste everything from [plugin/bracketed-paste.vim](https://github.com/ConradIrwin/vim-bracketed-paste/blob/master/plugin/bracketed-paste.vim) into your `~/.vimrc`.

Usage
=====

You need to be using a modern xterm-compatible terminal emulator that supports [bracketed paste mode](http://cirw.in/blog/bracketed-paste). xterm, urxvt, iTerm2, gnome-terminal (and other terminals using libvte), Putty (for Windows) are known to work.

Then whenever you are in the *insert mode* and paste into your terminal emulator using `command+v`, `shift+insert`, `ctrl+shift+v` or `middle-click`, vim will automatically `:set paste` for you.

Credit
======

The code for this plugin was taken from Chis Page's answer to a [StackOverflow question](http://stackoverflow.com/questions/5585129/pasting-code-into-terminal-window-into-vim-on-mac-os-x), I just packaged it.
