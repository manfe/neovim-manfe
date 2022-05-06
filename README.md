# Neovim - Manfe

Install neovim 0.8+

```
brew install --HEAD neovim
```

```
brew install watchman
brew install ripgrep  # https://github.com/BurntSushi/ripgrep#installation this is for telescope grep finder
brew install fd # https://github.com/sharkdp/fd#installation  this is for telescope grep finder
```

```
git clone git@github.com:manfe/neovim-manfe.git ~/.config/nvim
```

Run `nvim` and wait for the plugins to be installed 

**NOTE** (You will notice treesitter pulling in a bunch of parsers the next time you open Neovim) 

## Get healthy

Open `nvim` and enter the following:

```
:PackerSync
:checkhealth
:checkhealth telescope
```


You'll probably notice you don't have support for copy/paste also that python and node haven't been setup

So let's fix that

First we'll fix copy/paste

- On mac `pbcopy` should be builtin

- On Ubuntu

  ```
  sudo apt install xsel
  ```

- On Arch Linux

  ```
  sudo pacman -S xsel
  ```

Next we need to install python support (node is optional)

- Neovim python support

  ```
  pip install pynvim
  ```

- Neovim node support

  ```
  npm i -g neovim
  ```
---
