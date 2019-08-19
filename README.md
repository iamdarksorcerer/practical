# Practical Collection

## Table of Contents
* Environment
    * [Homebrew](#homebrew)
    * [Homebrew Cask](#homebrew-cask)
* Terminal
    * [ZSH](#zsh)
    * [Oh-My-Zsh](#oh-my-zsh)
* Editors
    * [Vim](#vim)
    * [Visual Studio Code](#visual-studio-code)
* Programming
    * [Git](#git)
    * [Python](#python)
    * [Go Lang](#go-lang)
    * [NVM](#nvm)
    * [NodeJS](#nodejs)
    * [Docker](#docker)
* Commands
    * [tree](#tree)
    * [htop](#htop)
    * [fzf](#fzf)  
* CLI shortcuts & tricks
    * [Create directory and navigate](#create-directory-and-navigate)
    * [Navigate to previous directory](#navigate-to-previous-directory)
    * [Run last command with `sudo`](#run-last-command-with-sudo)
## Environment
## Homebrew
> "Homebrew is a free and open-source software package management system that simplifies the installation of software on Apple's macOS operating system and Linux" - *[brew](https://brew.sh/)*  

Installation:  
```$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"```    
<sup>[&uarr;](#table-of-contents)</sup>

## Homebrew Cask
> "Cask is a project management tool for Emacs Lisp to automate the package development cycle; development, dependencies, testing, building, packaging and more" - *[cask](https://cask.readthedocs.io)*

Installation:  
```$ brew tap caskroom/cask```  
<sup>[&uarr;](#table-of-contents)</sup>

## Terminal
### ZSH
> "Zsh is a shell designed for interactive use, although it is also a powerful scripting language" - *[zsh](http://www.zsh.org)*
* Installation: 
```$ brew install zsh```
* Set as default shell:  
```$ sudo -s 'echo /usr/local/bin/zsh >> /etc/shells' && chsh -s /usr/local/bin/zsh```
* Plugins `(~/.zshrc)`:  
```plugins=(git zsh-syntax-highlighting)```  

<sup>[&uarr;](#table-of-contents)</sup>

### Oh-My-Zsh
> "A delightful community-driven (with 1,300+ contributors) framework for managing your zsh configuration. Includes 200+ optional plugins (rails, git, OSX, hub, capistrano, brew, ant, php, python, etc), over 140 themes to spice up your morning, and an auto-update tool so that makes it easy to keep up with the latest updates from the community" - *[oh-my-zsh](https://ohmyz.sh/)*

Installation:  
```$ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"```  
<sup>[&uarr;](#table-of-contents)</sup>

## Editors
### vim
> "Vim is a highly configurable text editor for efficiently creating and changing any kind of text. It is included as "vi" with most UNIX systems and with Apple OS X." - *[vim](https://www.vim.org/)*

Installation:  
```$ brew install vim```  
<sup>[&uarr;](#table-of-contents)</sup>

### Visual Studio Code
> "Visual Studio Code is a lightweight but powerful source code editor which runs on your desktop and is available for Windows, macOS and Linux. It comes with built-in support for JavaScript, TypeScript and Node.js and has a rich ecosystem of extensions for other languages (such as C++, C#, Java, Python, PHP, Go) and runtimes (such as .NET and Unity)." - *[Visual Studio Code](https://code.visualstudio.com/)*

Installation:  
```$ brew cask install visual-studio-code```  
<sup>[&uarr;](#table-of-contents)</sup>

### Sublime Text
> "Sublime Text is a proprietary cross-platform source code editor with a Python application programming interface (API). It natively supports many programming languages and markup languages, and functions can be added by users with plugins, typically community-built and maintained under free-software licenses." - *[Sublime Text](https://www.sublimetext.com/)*

Installation:  
```$ brew cask install sublime-text```  
<sup>[&uarr;](#table-of-contents)</sup>

## Programming
### Git
> "Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency." - *[git](https://git-scm.com/)*

Installation:  
```$ brew install git```  
<sup>[&uarr;](#table-of-contents)</sup>

### Python
> "Python is an interpreted, high-level, general-purpose programming language. Created by Guido van Rossum and first released in 1991, Python's design philosophy emphasizes code readability with its notable use of significant whitespace." - *[python](https://www.python.org/)*

Installation:  
* python3:  
```$ brew install python```  
* python2:  
```$ brew install python2```  

<sup>[&uarr;](#table-of-contents)</sup>

### Go Lang
> "Go is an open source programming language that makes it easy to build simple, reliable, and efficient software." - *[Go Lang](https://golang.org/)*

Installation:  
```$ brew install go```  
<sup>[&uarr;](#table-of-contents)</sup>

### NVM
> "Node Version Manager - POSIX-compliant bash script to manage multiple active node.js versions" - *[NVM](https://github.com/nvm-sh/nvm)*

Installation:  
```$ curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash```  
<sup>[&uarr;](#table-of-contents)</sup>

### NodeJS
> "Node.js® is a JavaScript runtime built on Chrome's V8 JavaScript engine." - *[NodeJS](https://nodejs.org)*

Installation:  
```$ nvm install node```  
<sup>[&uarr;](#table-of-contents)</sup>

### Docker
> "The Docker Platform is a set of integrated technologies and solutions for building, sharing and running container-based applications, from the developer’s desktop to the cloud." - *[Docker](https://www.docker.com)*

Installation:  
```$ brew cask install docker```  
<sup>[&uarr;](#table-of-contents)</sup>

## Commands
### tree
> "A recursive directory listing command or program that produces a depth-indented listing of files. It is available in Unix and Unix-like systems" - *[tree @ wiki](https://en.wikipedia.org/wiki/Tree_(command))*

Installation:  
```$ brew install tree```  
<sup>[&uarr;](#table-of-contents)</sup>

### htop
> " an interactive process viewer for Unix systems. It is a text-mode application (for console or X terminals) and requires ncurses" - *[htop](https://hisham.hm/htop/)*

Installation:  
```$ brew install htop```  
<sup>[&uarr;](#table-of-contents)</sup>

### fzf
> "Interactive Unix filter for command-line that can be used with any list; files, command history, processes, hostnames, bookmarks, git commits, etc." - *[fzf](https://github.com/junegunn/fzf)*

Installation:  
```$ brew install fzf```   
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
