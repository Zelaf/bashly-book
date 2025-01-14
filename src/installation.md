---
icon: terminal
order: 99
---

# Installation

Install bashly using one of these methods.

+++ Gem

If you have Ruby 3.0 or higher (`ruby -v`), use this installation method:

```shell
gem install bashly
```

+++ Homebrew

Mac users can enable Ruby gem installation first, and then install bashly:

```shell
brew install brew-gem
brew gem install bashly
```

+++ Docker

If you have docker installed, you can create an alias that will run the docker image:

```shell
alias bashly='docker run --rm -it --user $(id -u):$(id -g) --volume "$PWD:/app" dannyben/bashly'
```

+++


## Bash Completions

To enable bash completions for the `bashly` executable itself run:

```shell
bashly completions --install
```

You might need to install the `bash-completion` package for your operating
system if it is not already installed. For example:

```shell
brew install bash-completion
# or
sudo apt install bash-completion
```

!!!success Tip
To generate bash completions for your own scripts, see  
[Advanced Features :icon-chevron-right: Bash Completion](/advanced/bash-completion/)
!!!

## Prerequisites

The bash scripts generated by bashly can run in any shell, but require that
**bash 4 or higher** is installed.

Mac users can upgrade bash by running:

```
brew install bash
```
