# Table of Contents

* Environment
    * [Homebrew](#homebrew)
    * [Homebrew Cask](#homebrew-cask)
* Terminal
    * [iTerm2](#iterm2)
    * [Fonts](#fonts)
    * [iTerm Themes](#iterm2-themes)
    * [ZSH](#zsh)
    * [Oh-My-Zsh](#oh-my-zsh)
    * [Oh-My-Zsh plugins](#oh-my-zsh-plugins)
        * [zsh-syntax-highlighting](#zsh-syntax-highlighting)
        * [z](#z)
* Text Editors
    * [vim](#vim)
    * [neovim](#neovim/nvim)
    * [Visual Studio Code](#visual-studio-code)
* Programming
    * [Git](#git)
    * [Python](#python)
    * [Go Lang](#go-lang)
    * [NVM](#nvm)
    * [NodeJS](#nodejs)
    * [Docker](#docker)
    * [Java (OpenJDK)](#java-openjdk)
    * [Groovy (sdk)](#groovy-sdk)
* CLI Commands
    * [tree](#tree)
    * [htop](#htop)
    * [fzf](#fzf)
    * [jq](#jq)
    * [bat](#bat)
    * [axe](#axe)
    * [delta](#delta)
    * [httpie](#httpie)
    * [httpstat](#httpstat)
* CLI shortcuts & tricks
    * [Create directory and navigate](#create-directory-and-navigate)
    * [Navigate to previous directory](#navigate-to-previous-directory)
    * [Run last command with `sudo`](#run-last-command-with-sudo)
    * [Create file backup](#create-file-backup)
    * [Repeat command like last execution](#repeat-command-like-last-execution)

## Environment

## Homebrew

> "Homebrew is a free and open-source software package management system that  
simplifies the installation of software on Apple's macOS operating system and  
Linux" - *[brew](https://brew.sh/)*  

Installation:  
```$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"```  
<sup>[&uarr;](#table-of-contents)</sup>

## Homebrew Cask

> "Cask is a project management tool for Emacs Lisp to automate the package  
development cycle; development, dependencies, testing, building, packaging and  
more" - *[cask](https://cask.readthedocs.io)*

Installation:  
```$ brew tap caskroom/cask```  
<sup>[&uarr;](#table-of-contents)</sup>

## Terminal

### iTerm2

> "iTerm2 is a replacement for Terminal and the successor to iTerm. It works  
on Macs with macOS 10.12 or newer. iTerm2 brings the terminal into the modern  
age with features you never knew you always wanted." - *[iTerm2](https://www.iterm2.com/)*

Installation:  
```$ brew cask install iterm2```  
<sup>[&uarr;](#table-of-contents)</sup>

### Fonts

Installation:  
```$ brew tap caskroom/fonts```  
```$ brew cask install font-source-code-pro font-roboto font-fira-code font-inconsolata\```  
```font-droidsansmono-nerd-font font-firacode-nerd-font font-hermit-nerd-font\```  
```font-inconsolata-nerd-font font-liberationmono-nerd-font font-monofur-nerd-font\```  
```font-mononoki-nerd-font font-mplus-nerd-font font-robotomono-nerd-font\```  
```font-ubuntumono-nerd-font font-sourcecodepro-nerd-font font-inconsolata-nerd-font\```  
```font-office-code-pro```  

Additional:
*[JetBrains Mono font](https://github.com/JetBrains/JetBrainsMono)*

```bash
$ brew tap homebrew/cask-fonts
$ brew cask install font-jetbrains-mono
```

<sup>[&uarr;](#table-of-contents)</sup>

### iTerm2 Themes

Installation:  

* Visit [iTerm2-Color-Schemes](https://github.com/mbadolato/iTerm2-Color-Schemes) and download themes folder or clone repository
* Follow [installation](https://github.com/mbadolato/iTerm2-Color-Schemes#installation-instructions) instructions  

<sup>[&uarr;](#table-of-contents)</sup>

### ZSH

> "Zsh is a shell designed for interactive use, although it is also a powerful scripting language" - *[zsh](http://www.zsh.org)*

* Installation:  
```$ brew install zsh```
* Set as default shell:  
```$ sudo -s 'echo /usr/local/bin/zsh >> /etc/shells' && chsh -s /usr/local/bin/zsh```

<sup>[&uarr;](#table-of-contents)</sup>

### Oh-My-Zsh

> "A delightful community-driven (with 1,300+ contributors) framework for  
managing your zsh configuration. Includes 200+ optional plugins (rails, git,  
OSX, hub, capistrano, brew, ant, php, python, etc), over 140 themes to spice  
up your morning, and an auto-update tool so that makes it easy to keep up with  
the latest updates from the community" - *[oh-my-zsh](https://ohmyz.sh/)*

Installation:  
```$ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"```  
<sup>[&uarr;](#table-of-contents)</sup>

### Oh-My-Zsh plugins

In order to enable/disable oh-my-zsh plugins, open the `(~/.zshrc)` file and  
adjust following line:  
```plugins=([plugins])```  

#### zsh-syntax-highlighting

> "This package provides syntax highlighting for the shell zsh. It enables  
highlighting of commands whilst they are typed at a zsh prompt into an  
interactive terminal. This helps in reviewing commands before running them,  
particularly in catching syntax errors" - *[zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)*

* Installation:  
```$ brew install zsh-syntax-highlighting```  
OR  
```$ git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting```
* Activate the plugin in `~/.zshrc`:  
```$ plugins=( [plugins...] zsh-syntax-highlighting)```
Note: `zsh-syntax-highlighting` should be last plugin enabled  
<sup>[&uarr;](#table-of-contents)</sup>

#### z

> "Tracks most-used directories to make cd smarter" - *[z](https://github.com/rupa/z)*

* Installation:  
 ```$ brew install z```  
* Setup:  
Add either:
    * `[ -f $(brew --prefix)/etc/profile.d/z.sh ] && source $(brew --prefix)/etc/profile.d/z.sh`  
    OR  
    * `. /usr/local/etc/profile.d/z.sh`  
    to your `~/.zshrc`  

<sup>[&uarr;](#table-of-contents)</sup>

## Text Editors

### vim

> "Vim is a highly configurable text editor for efficiently creating and  
changing any kind of text. It is included as "vi" with most UNIX systems  
and with Apple OS X." - *[vim](https://www.vim.org/)*

Installation:  
```$ brew install vim```  
<sup>[&uarr;](#table-of-contents)</sup>

### neovim/nvim

> "Hyperextensible Vim-based text editor" - *[neovim](https://github.com/neovim/neovim)*

Installation:  

```$ brew install neovim```

Additional:  

```bash
alias vim="nvim"
alias vi="nvim"
```

<sup>[&uarr;](#table-of-contents)</sup>

### Visual Studio Code

> "Visual Studio Code is a lightweight but powerful source code editor which  
runs on your desktop and is available for Windows, macOS and Linux. It comes  
with built-in support for JavaScript, TypeScript and Node.js and has a rich  
ecosystem of extensions for other languages (such as C++, C#, Java, Python,  
PHP, Go) and runtimes (such as .NET and Unity)." - *[Visual Studio Code](https://code.visualstudio.com/)*

Installation:  
```$ brew cask install visual-studio-code```  
<sup>[&uarr;](#table-of-contents)</sup>

### Sublime Text

> "Sublime Text is a proprietary cross-platform source code editor with a  
Python application programming interface (API). It natively supports many  
programming languages and markup languages, and functions can be added by  
users with plugins, typically community-built and maintained under  
free-software licenses." - *[Sublime Text](https://www.sublimetext.com/)*

Installation:  
```$ brew cask install sublime-text```  
<sup>[&uarr;](#table-of-contents)</sup>

## Programming

### Git

> "Git is a free and open source distributed version control system designed  
to handle everything from small to very large projects with speed and  
efficiency." - *[git](https://git-scm.com/)*

Installation:  
```$ brew install git```  
<sup>[&uarr;](#table-of-contents)</sup>

### Python

> "Python is an interpreted, high-level, general-purpose programming language.  
Created by Guido van Rossum and first released in 1991, Python's design  
philosophy emphasizes code readability with its notable use of significant  
whitespace." - *[python](https://www.python.org/)*

Installation:  

* python3:  
```$ brew install python```  
* python2:  
```$ brew install python2```  

<sup>[&uarr;](#table-of-contents)</sup>

### Go Lang

> "Go is an open source programming language that makes it easy to build simple,  
reliable, and efficient software." - *[Go Lang](https://golang.org/)*

Installation:  
```$ brew install go```  
<sup>[&uarr;](#table-of-contents)</sup>

### NVM

> "Node Version Manager - POSIX-compliant bash script to manage multiple active  
node.js versions" - *[NVM](https://github.com/nvm-sh/nvm)*

Installation:  
```$ curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash```  
<sup>[&uarr;](#table-of-contents)</sup>

### NodeJS

> "Node.js® is a JavaScript runtime built on Chrome's V8 JavaScript engine." - *[NodeJS](https://nodejs.org)*

Installation:  
```$ nvm install node```  
<sup>[&uarr;](#table-of-contents)</sup>

### Docker

> "The Docker Platform is a set of integrated technologies and solutions for  
building, sharing and running container-based applications, from the  
developer’s desktop to the cloud." - *[Docker](https://www.docker.com)*

Installation:  
```$ brew cask install docker```  
<sup>[&uarr;](#table-of-contents)</sup>

### Java (OpenJDK)

> "OpenJDK (Open Java Development Kit) is a free and open-source implementation  
of the Java Platform, Standard Edition (Java SE). It is the result of an effort  
Sun Microsystems began in 2006. The implementation is licensed under the GNU  
General Public License (GNU GPL) version 2 with a linking exception. Were it  
not for the GPL linking exception, components that linked to the Java class  
library would be subject to the terms of the GPL license. OpenJDK is the  
official reference implementation of Java SE since version 7" - *[Open JDK @ wiki](https://en.wikipedia.org/wiki/OpenJDK)*

Installation:  
```$ brew cask install adoptopenjdk```  
<sup>[&uarr;](#table-of-contents)</sup>

### Groovy (SDK)

> "Apache Groovy is a powerful, optionally typed and dynamic language, with  
static-typing and static compilation capabilities, for the Java platform aimed  
at improving developer productivity thanks to a concise, familiar and easy to  
learn syntax. It integrates smoothly with any Java program, and immediately  
delivers to your application powerful features, including scripting  
capabilities, Domain-Specific Language authoring, runtime and compile-time  
meta-programming and functional programming." - *[Groovy Lang](http://groovy-lang.org)*  

Installation:  

* ```$ brew install groovysdk```  
* OPTIONAL: In order to set `GROOVY_HOME` environment variable, add ```export GROOVY_HOME="/usr/local/opt/groovysdk/libexec"``` to your `.zshrc` / `.bashrc`

<sup>[&uarr;](#table-of-contents)</sup>

## CLI Commands

### tree

> "A recursive directory listing command or program that produces a  
depth-indented listing of files. It is available in Unix and Unix-like systems" - *[tree @ wiki](https://en.wikipedia.org/wiki/Tree_(command))*

Installation:  
```$ brew install tree```  
<sup>[&uarr;](#table-of-contents)</sup>

### htop

> "An interactive process viewer for Unix systems. It is a text-mode  
application (for console or X terminals)" - *[htop](https://hisham.hm/htop/)*

Installation:  
```$ brew install htop```  
<sup>[&uarr;](#table-of-contents)</sup>

### fzf

> "Interactive Unix filter for command-line that can be used with any list;  
files, command history, processes, hostnames, bookmarks, git commits, etc" - *[fzf](https://github.com/junegunn/fzf)*

Installation:  
```$ brew install fzf```  
<sup>[&uarr;](#table-of-contents)</sup>

### jq

> "jq is like sed for JSON data - you can use it to slice and filter and map  
and transform structured data with the same ease that sed, awk, grep and  
friends let you play with text" - *[jq](https://stedolan.github.io/jq/)*

Installation:  
```$ brew install jq```  
<sup>[&uarr;](#table-of-contents)</sup>

### bat

> "A cat(1) clone with syntax highlighting and Git integration." - *[bat](https://github.com/sharkdp/bat)*

Installation:  
```$ brew install bat```  

Additional:  

```bash
alias cat='bat'
```

<sup>[&uarr;](#table-of-contents)</sup>

### exa

> "exa is a replacement for ls written in Rust." - *[exa](https://github.com/ogham/exa)*  

Installation:  
```$ brew install exa```  

Additional:  

```bash
alias la='ls -alh --git'
alias ls='exa'
```

<sup>[&uarr;](#table-of-contents)</sup>

### delta

> "A viewer for git and diff output" - *[delta](https://github.com/dandavison/delta)*

Installation:  
```brew install git-delta```  

Additional:  
Add to your `~/.gitconfig`:

```gitconfig
[core]
    pager = delta

[interactive]
    diffFilter = delta --color-only

[delta]
    features = side-by-side line-numbers decorations
    syntax-theme = Monokai Extended


[delta "decorations"]
    commit-decoration-style = bold yellow box ul
    file-style = bold yellow ul
    file-decoration-style = none
```

### httpie

> "HTTPie: a CLI, cURL-like tool for humans" - *[httpie](https://github.com/jakubroztocil/httpie)*

Installation:  
```$ brew install httpie```  
<sup>[&uarr;](#table-of-contents)</sup>

### httpstat

> "httpstat visualizes curl statistics. It tells you where did your request spend time." - *[httpstat](https://github.com/reorx/httpstat)*  

Installation:  
```$ brew install httpstat```  
<sup>[&uarr;](#table-of-contents)</sup>

## CLI shortcuts & tricks

### Create directory and navigate

```$ mkdir <name> && cd $_```  
<sup>[&uarr;](#table-of-contents)</sup>

### Navigate to previous directory

```$  cd -```  
<sup>[&uarr;](#table-of-contents)</sup>

### Run last command with sudo

```$  sudo !!```  
<sup>[&uarr;](#table-of-contents)</sup>

### Create file backup

```$ cp /path/to/file.txt{,.bkp}```  
<sup>[&uarr;](#table-of-contents)</sup>

### Repeat command like last execution

Fast repeat of last run with same arguments  
```$ !<command>```  

<sup>[&uarr;](#table-of-contents)</sup>
