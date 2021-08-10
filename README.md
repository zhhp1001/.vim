# zhhp's Vim configuration

```bash
cd ~
git clone https://github.com/zhhp1001/.vim.git
```

# vim plugin



## Dependency

### Vim-plug

```bash
curl -fLo ~/.vim/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

### Nodejs
> you can use nvm too...
```bash
curl -sL install-node.now.sh/lts | bash
```

## Install plug

```bash
$ vim		#open vim
$ :PlugInstall # install plugs
```

### clangd (for C/C++)

> https://clangd.llvm.org/installation.html

### coc-clangd

in vim, run `:CocInstall coc-clangd`

`coc-clangd` will try to find `clangd` from your `$PATH`, if not found, you can run `:CocCommand clangd.install` to install the [latest release](https://github.com/clangd/clangd/releases) from GitHub

> https://github.com/clangd/coc-clangd

## bear make generate `complie_commands.json`

`sudo apt install bear`

Use `bear make` instead of `make` 

The output file called `compile_commands.json` is saved in the current directory. 

`coc-nvim` will use this file to navigate source code.

> https://github.com/rizsotto/Bear
