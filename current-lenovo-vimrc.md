---
title: current-lenovo-vimrc
date: 2024-07-09
tags: 
---
# current-lenovo-vimrc
set nocompatible   " Don't try to be vi compatible
filetype off   " Helps force plugins to load correctly when it is turned back on below
syntax on    " Turn on syntax highlighting
filetype plugin indent on   " For plugins to load correctly
" TODO: Pick a leader key
" let mapleader = ","
"
set modelines=0     " Security
set number    " Show line numbers
set ruler  " Show file stats
set visualbell   " Blink cursor on error instead of beeping (grr)
set encoding=utf-8  " Encoding
" set wrap  " Whitespace
" set textwidth=79
set formatoptions=tcqrn1
set tabstop=2
set shiftwidth=2
set softtabstop=2
set expandtab
set noshiftround
set linebreak " Wraps text at the end of a word. ...
set nolist " You must turn off list which displays whitespace characters as text.
set linebreak
set nolist
set spell
set scrolloff=3   " Cursor motion
set backspace=indent,eol,start
set matchpairs+=<:> " use % to jump between pairs
" runtime! macros/matchit.vim
" Move up/down editor lines
nnoremap j gj
nnoremap k gk
set hidden   " Allow hidden buffers
set ttyfast   " Rendering
set laststatus=2   " Status bar
set showmode   " Last line
set showcmd

" Searching
"nnoremap / /\v
"vnoremap / /\v
set hlsearch
set incsearch
set ignorecase
set smartcase
set showmatch
map <leader><space> :let @/=''<cr> " clear search

" Remap help key.
inoremap <F1> <ESC>:set invfullscreen<CR>a
