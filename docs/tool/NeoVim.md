# NeoVim

更强大的 Vim。



## 安装

为了更好的显示效果，最好使用 Nerd fonts 字体，Nerd fonts 并不是一种新的字体，而是把常用的图标以打补丁的方式打到常用的字体上。在 Nerd fonts 的官方仓库上，可以找到打了补丁的常用字体，这里使用 jetbrains mono 字体，在 `https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts/JetBrainsMono` 下载打好了补丁的字体，安装该字体并设置后，就可以在命令行中显示一些小图标了。

我当前使用的环境是 Ubuntu20.04，所以使用 apt 安装 neovim：

```bash
sudo add-apt-repository ppa:neovim-ppa/unstable
sudo apt update
sudo apt install neovim
```

安装成功后，运行 `nvim --version` 命令，确认 nvim 版本在 0.7 以上。现在可以用 nvim 来替代 vim 了，编辑 `~/.bashrc` 文件，添加别名：

```bash
alias vim='nvim'
alias vi='nvim'
alias v='nvim'
```

保存后用 `source` 命令运行刚刚编辑的文件，改变环境变量，这样无论运行 vim、vi 还是 v 打开的都是 nvim 了。

nvim 最大的亮点就是高度可配置，通过各种配置与插件可以让 nvim 媲美强大的 IDE。nvim 的配置文件在 `~/.config/nvim` 目录下。首先在该目录下新建一个 lua 文件——`init.lua`，这是整个配置的入口文件，负责引用所有其他模块，基本上想要打开或者关闭某个插件只要在这里修改即可。最后在该目录新建一个 `lua` 目录，用来存放将来的配置、插件等 lua 脚本文件。

