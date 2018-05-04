==Install gVim==
1. Run install as Admin
2. Full install
3. Install to default location
4. Move vimfiles and _vimrc from C:\Program Files(x86)\Vim to ~\
5. Delete all folders in ~\vimfiles
6. Move C:\Program Files(x86)\vimXX\autoload to ~\vimfiles

==Install Vundle plugin manager==
1. Create bundle directory in ~\vimfiles
2. Install Chocolatey
3. Follow Vundle for Windows setup instructions: https://github.com/VundleVim/Vundle.vim/wiki/Vundle-for-Windows
4. Copy example vimrc https://github.com/VundleVim/Vundle.vim
5. Replace 
    set rtp+=~/.vim/bundle/Vundle.vim
    call vundle#begin()
  with
    set rtp+=$HOME/vimfiles/bundle/Vundle.vim/
    call vundle#begin('$HOME/vimfiles/bundle/')
6. Run :PluginInstall

