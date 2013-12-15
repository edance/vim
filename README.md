# Installing on your own machine

    cd ~
    git clone http://github.com/edance/vim.git ~/.vim
    ln -s ~/.vim/vimrc ~/.vimrc
    ln -s ~/.vim/gvimrc ~/.gvimrc
    cd ~/.vim
    git submodule update --init 

## Installing plugins as git submodules

    cd ~/.vim
    mkdir ~/.vim/bundle
    git submodule add http://github.com/tpope/vim-fugitive.git bundle/fugitive
    git add .
    git commit -m "Install Fugitive.vim bundle as a submodule."

## Upgrading all bundled plugins
    git submodule foreach git pull origin master

# Big Thanks to zjrosen1 ;)
