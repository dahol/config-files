# Config-files

## Install

### Clone git repo

`git clone https://github.com/dahol/config-files`

### Backup current config (if exists)
<<<<<<< HEAD

```
current=~/.config/init.vim
if current -f "$current"; then
    cp ~/.config/init.vim ~/.config/init.vim.bk
fi
```
=======
>>>>>>> 76033a3f92c40063e4c2801a61eff65f0aee4dfd

`cp ~/.config/init.vim ~/.config/init.vim.bk`

### Create nvim-folder if it does not exist

`mkdir -p ~/.config/nvim/`

### Copy new config

`cp config-files/init.vim ~/.config/nvim/init.vim`

### Install plug-vim

`sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'`

### Install plugin selection

`:Pluginstall`
