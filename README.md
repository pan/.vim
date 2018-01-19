## .vim
My own VIM config & plugins for development that can be deployed quickly to new machines.
### installation
```
$ git clone https://github.com/pan/.vim
$ cd .vim
$ git submodule update --init

### documentation
```
cd .vim/bundle
vim -u NONE -c "helptags vim-rails/doc" -c q
