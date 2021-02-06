# Setup neovim on new maschine

## Install neovim, nodejs, python, etc
```
sudo apt update
sudo apt install neovim python3 python3-pip nodejs npm -y
```

### Install python modules for neovim
```
pip3 install pynvim
npm i -g neovim
```

```
pip3 install neovim-remote
```

This will install `nvr` to `~/.local/bin` so you will need to add the following to your `bashrc` or `zshrc`.
```
export PATH=$HOME/.local/bin:$PATH
```

## Install nvim Plugins
Run the following commands inside nvim
```
nvim
:PlugInstall
:UpdateRemotePlugins
:q
```

## Check health of nvim installation
Run the following command inside nvim
```
:checkhealth
```
Python 3 and Nodejs provider must be `OK`. ruby, python2, etc are optional.

## Install extensions for programming languages using Coc
Run the following commands inside nvim

For generic web-development:
```
:CocInstall coc-tsserver coc-json coc-html coc-css
```

For Python:
```
:CocInstall coc-python
```

For PHP:
```
:CocInstall coc-phpls
```

[more extensions](https://github.com/neoclide/coc.nvim/wiki/Using-coc-extensions)
