# Config-files

## Install

### Clone git repo

`git clone https://github.com/dahol/config-files`

### Backup current config (if exists)

`cp ~/.config/init.vim ~/.config/init.vim.bk`

### make sure dir exists

`mkdir -p ~/.config/nvim/`

### Copy new config

`cp config-files/init.vim ~/.config/nvim/init.vim`

### Install plug-vim

`sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'`

### Install plugin selection

:Pluginstall

### Cleanup

`rm -d -r config-files/`
