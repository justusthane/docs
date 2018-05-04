==Install gVim==
- Run install as Admin
- Full install
- Install to default location
- Move vimfiles and _vimrc from C:\Program Files(x86)\Vim to ~\
- Delete all folders in ~\vimfiles
- Move C:\Program Files(x86)\vimXX\autoload to ~\vimfiles

==Install Vundle plugin manager==
- Create bundle directory in ~\vimfiles
- Install Chocolatey
- Follow Vundle for Windows setup instructions: https://github.com/VundleVim/Vundle.vim/wiki/Vundle-for-Windows
- Copy example vimrc https://github.com/VundleVim/Vundle.vim
- Replace 
    set rtp+=~/.vim/bundle/Vundle.vim
    call vundle#begin()
  with
    set rtp+=$HOME/vimfiles/bundle/Vundle.vim/
    call vundle#begin('$HOME/vimfiles/bundle/')
- Run :PluginInstall

