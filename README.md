# configs

## PS1
```
export PS1='\[\033[0;32m\]\[\033[0m\033[0;32m\][\u\[\033[0;36m\]@\w\[\033[0;32m\]]-[$(git branch 2>/dev/null | grep "^*" | colrm 1 2)\[\033[0;32m\]]\[\033[0m\033[0;32m\] \$\[\033[0m\033[0;32m\]\[\033[0m\] '
```

## VIM
### Install DirDiff
https://github.com/will133/vim-dirdiff
### Install NerdTree
https://github.com/will133/vim-dirdiff
### .vimrc
```
execute pathogen#infect()
syntax on
filetype plugin indent on

autocmd vimenter * NERDTree
autocmd bufenter * if (winnr("$") == 1 && exists("b:NERDTree") && b:NERDTree.isTabTree()) | q | endif

set wildchar=<Tab> wildmenu wildmode=full
set wildcharm=<C-Z>
nnoremap <F9> :b <C-Z>

set number
set ignorecase
set tabstop=8 softtabstop=0 expandtab shiftwidth=4 smarttab
set showmatch 
set ruler
```
