### 安装 homebrew
~~~bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
~~~

### 安装 iterm2
~~~bash
brew install iterm2
~~~

### 安装 zsh
~~~bash
brew install zsh
~~~

### 安装 fzf
~~~bash
brew install fzf
$(brew --prefix)/opt/fzf/install
~~~

### 安装thefuck
~~~bash
brew install thefuck
~~~

### 安装 tmux
~~~bash
brew install tmux
cd ~ && git clone https://github.com/gpakosz/.tmux.git
ln -s -f .tmux/.tmux.conf
cp .tmux/.tmux.conf.local .
~~~

### 安装字体 PowerlineSymbols.otf

### 编辑 ~/.zshrc
~~~bash
source ~/.profile
export ZSH=~/.oh-my-zsh
source $ZSH/oh-my-zsh.sh
[ -f ~/.fzf.zsh ] && source ~/.fzf.zsh
~~~

### 编辑 ~/.profile
~~~bash
export LANG=en_US.UTF-8

export PATH=/usr/local/bin
export PATH=$PATH:/usr/bin:/usr/sbin
export PATH=$PATH:/bin
export PATH=$PATH:/sbin
export PATH=$PATH:/usr/local/sbin
export PATH=$PATH:/usr/X11/bin

# PS COLOR
export CLICOLOR=1
export LSCOLORS=gxfxcxdxbxegedabagacad
export PS1='\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;36m\]\w\[\033[00m\]\$'
export TERM=screen-256color-bce


alias tmux="tmux -2"
alias W="tmux -2 attach || tmux"

# fuck
eval $(thefuck --alias)

# other env

~~~
