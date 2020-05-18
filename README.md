# 환경 세팅

## .bash
bashrc
```

PS1='[\[\033[01;31m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[00m\]] \n$ '
# User specific aliases and functions

alias l.='ls -d .* --color=auto'
alias ll='ls -lhX --color=auto'
alias ls='ls  --color=auto'
alias rm='rm -i'
alias cp='cp -i'
alias mv='mv -i'
alias vi='/bin/vim'

# Source global definitions
if [ -f /etc/bashrc ]; then
	. /etc/bashrc
fi

# ls color 
export LS_COLORS='di=1;5;92:fi=37:ln=36:pi=5:so=5:bd=5:cd=5:or=31:mi=93:ex=35:*.rpm=90'

```

## .exrc
```
set nu
set tabstop=2
set shiftwidth=2
set ai
```
## .vimrc 

```
set history=256
" line number
set nu
" tab size
set tabstop=2
set softtabstop=2
set smarttab
set expandtab
" shift size
set shiftwidth=2
" indent
set autoindent
set cindent
set smartindent
" last modified point
au BufReadPost *
\ if line("'\"") > 0 && line("'\"") <= line("$") |
\ exe "norm g`\"" |
\ endif
" Syntax Highlighting
syntax on
" status 
set laststatus=2
set statusline=\ %<%l:%v\ [%P]%=%a\ %h%m%r\ %F\
" search highlight
set hlsearch 
set incsearch
set ignorecase
" {}
set showmatch
" current cursor point
set ruler
"set paste

"colorscheme darkblue
colorscheme set
```
