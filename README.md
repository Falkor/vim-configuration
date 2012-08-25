# My Vim Configuration (so-called 'Ultimate' by Evan Coury)

Based on the [Ultimate Vim Configuration](https://github.com/EvanDotPro/vim-configuration) Version 1.0.0 created by Evan Coury

```
             _____     _ _              _     
            |  ___|_ _| | | _____  _ __( )___ 
            | |_ / _` | | |/ / _ \| '__|// __|
            |  _| (_| | |   < (_) | |    \__ \
            |_|  \__,_|_|_|\_\___/|_|    |___/
            _                              __ _
           (_)                            / _(_)
     __   ___ _ __ ___     ___ ___  _ __ | |_ _  __ _
     \ \ / / | '_ ` _ \   / __/ _ \| '_ \|  _| |/ _` |
      \ V /| | | | | | | | (_| (_) | | | | | | | (_| |
       \_/ |_|_| |_| |_|  \___\___/|_| |_|_| |_|\__, |
                                                 __/ |
                                                |___/
```

## Introduction

This is my personal vim config. 
Nearly all credit goes to Evan Coury (aka EvanDotPro) so prefer to use its 
[Ultimate Vim Configuration](https://github.com/EvanDotPro/vim-configuration) rather than this one as it 
integrates only a few changes to suit my tastes.

Below are the initial text from Evan.  

## Evan's notes

Author: Evan Coury, http://blog.evan.pro/
URL: https://github.com/EvanDotPro/vim-configuration

Special thanks to:

- Steve Francia for [spf13-vim](https://github.com/spf13/spf13-vim)
- Marc Weber for [Vundle](https://github.com/gmarik/vundle)
- [Aleksey Khudyakov](https://github.com/Xerkus) (aka Xerkus) for adding git-treeish support to Vundle
- All of the authors of the other amazing Vim plugins I use every day.

## Installation (Linux & Mac)

- If you have an existing vim configuration, back it up:
    - `for i in $HOME/.vim $HOME/.vimrc $HOME/.gvimrc; do [ -e $i ] && mv $i $i.\`date +%Y%m%d\`; done`
- `git clone --recursive https://github.com/EvanDotPro/vim-configuration.git $HOME/edp-vim`
- `ln -s $HOME/edp-vim $HOME/.vim`
- `ln -s $HOME/edp-vim/.vimrc $HOME/.vimrc`
- `vim +BundleInstall! +BundleClean +q`

## Features

### Base Customizations

This config ships with the following basic customizations for vim:

* `:w!!` invokes a write with sudo.
* Trailing whitespace is highlighted in red.
* Trailing whitespace is automatically removed when saving c, cpp, java, php, javascript, python, twig, xml, yml, phtml, or vimrc files.
* Tab characters displayed as ▸
* Make searching highlighted, incremental, and case insensitive unless a capital letter is used.
* Gvim gui cleaned up (removes menu bars and buttons).
* `F1` is mapped to <Esc> to prevent accidental opening of help.
* `;` is remapped to `:` for easier transition into command mode.
* The Vim backup, swap, and view files are consolidated in one place so they do not interfere with your workspace.

### Fully Customizable

This configuration is fully customizable
If you want to customize the config, you should not need to fork and/or make changes directly to the `.vimrc`. Instead, you can simply create an `override.local.vim` file in your vim directory and override any settings there.

### Easy Shortcuts

* `<C-a>` - Select all
* `<leader>w` - Write current file
* `<leader>c` and `<leader>v` - Copy and paste with the system clipboard

## Plugins

* **General**
    - [NERDTree](https://github.com/scrooloose/nerdtree)
    - [NERDTree-symlink](EvanDotPro/nerdtree-symlink) (small plugin by me to allow easily creating symlinks from NERDTree.
    - [ctrlp.vim](https://github.com/kien/ctrlp.vim)
    - [Powerline](https://github.com/Lokaltog/vim-powerline)
    - [numbers.vim](http://myusuf3.github.com/numbers.vim/)
    - [FuzzyFinder](https://github.com/vim-scripts/FuzzyFinder) (and dependency [L9](https://github.com/vim-scripts/L9))
* **Themes**
    - [Lucius](https://github.com/vim-scripts/Lucius) (default)
    - [Solarized](https://github.com/altercation/vim-colors-solarized)
    - [vim-colors](https://github.com/spf13/vim-colors) (contains a ton of additional themes)
* **General Programming**
    - [fugitive](https://github.com/tpope/vim-fugitive)
    - [tabular](https://github.com/godlygeek/tabular)
    - [syntastic](https://github.com/scrooloose/syntastic)
    - [gist-vim](https://github.com/mattn/gist-vim) (and dependency [webapi-vim](https://github.com/mattn/webapi-vim))

(TODO: There's more -- I need to finish this list)
