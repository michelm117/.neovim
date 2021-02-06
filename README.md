# Setup neovim on new maschine

## Install neovim, nodejs, python, etc
```
sudo apt update
sudo apt install neovim python3 python3-pip nodejs npm -y


```

### Install python modules for neovim
```
pip install pynvim
npm i -g neovim
curl -sL install-node.now.sh | sh
```

```
pip install neovim-remote
```
This will install `nvr` to `~/.local/bin` so you will need to add the following to your `bashrc` or `zshrc`.
```
export PATH=$HOME/.local/bin:$PATH
```
