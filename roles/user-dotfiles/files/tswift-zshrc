#!/usr/local/bin/zsh

export ZSH=$HOME/.oh-my-zsh
ZSH_THEME="blusch"
COMPLETION_WAITING_DOTS="true"
DISABLE_UNTRACKED_FILES_DIRTY="true"

plugins=(
    autojump
    bower
    brew
    cpv
    django
    gem
    git
    gitignore
    history
    hub
    lol
    nvm
    nyan
    pip
    pyenv
    osx
    python
    rbenv
    rsync
    ruby
    sublime
    svn
    terminalapp
    vagrant
    virtualenv
    zsh_reload
)

# nvm # must be set before nvm plugin is loaded
export NVM_DIR=~/.nvm

source $ZSH/oh-my-zsh.sh

# User configuration
CLASSPATH=$HOME/workspace/libs
export CLASSPATH

# Python
export PYTHONSTARTUP=~/.pythonrc

# pyenv
export PYENV_ROOT=/usr/local/opt/pyenv
which pyenv > /dev/null && eval "$(pyenv init -)"

# rbenv
export RBENV_ROOT=/usr/local/var/rbenv
which rbenv > /dev/null && eval "$(rbenv init -)"

# autoenv
[[ -d /usr/local/opt/autoenv ]] && source /usr/local/opt/autoenv/activate.sh

# git
touch ~/.git-completion
source ~/.git-completion

# Aliases
touch ~/.aliases
source ~/.aliases

# Secret stuff goes in here so you can't see it
touch ~/.secrets
source ~/.secrets

PATH=$HOME/bin:$PATH
PATH=/usr/local/sbin:$PATH
PATH=/opt/chefdk/bin:$PATH
PATH=/usr/local/bin:$PATH
export PATH

# added by travis gem
[ -f /Users/blue/.travis/travis.sh ] && source /Users/blue/.travis/travis.sh

export R29=~/workspace/r29
export ws=~/workspace

touch ~/.todo
cat ~/.todo

[ -f ~/.fzf.zsh ] && source ~/.fzf.zsh
