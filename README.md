# configs

# PS1
```
export PS1='\[\033[0;32m\]\[\033[0m\033[0;32m\][\u\[\033[0;36m\]@\w\[\033[0;32m\]]-[$(git branch 2>/dev/null | grep "^*" | colrm 1 2)\[\033[0;32m\]]\[\033[0m\033[0;32m\] \$\[\033[0m\033[0;32m\]\[\033[0m\] '
```
