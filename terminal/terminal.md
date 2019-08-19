# Terminal

* homebrew:  
    > "Homebrew is a free and open-source software package management system that simplifies the installation of software on Apple's macOS operating system and Linux" - *[brew](https://brew.sh/)*

    ```$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"```
* home brew cask:  
    > "Cask is a project management tool for Emacs Lisp to automate the package development cycle; development, dependencies, testing, building, packaging and more" - *[cask](https://cask.readthedocs.io)*

    ```$ brew tap caskroom/cask```  
* zsh: 
    > "Zsh is a shell designed for interactive use, although it is also a powerful scripting language" - *[zsh](http://www.zsh.org)*
    * Install:  
    ```$ brew install zsh```
    * Set as default shell:  
    ```$ sudo -s 'echo /usr/local/bin/zsh >> /etc/shells' && chsh -s /usr/local/bin/zsh```
    * Plugins:  
    ```plugins=(git zsh-syntax-highlighting)```
* oh-my-zsh:  
    > "A delightful community-driven (with 1,300+ contributors) framework for managing your zsh configuration. Includes 200+ optional plugins (rails, git, OSX, hub, capistrano, brew, ant, php, python, etc), over 140 themes to spice up your morning, and an auto-update tool so that makes it easy to keep up with the latest updates from the community" - *[oh-my-zsh](https://ohmyz.sh/)*

    ```$ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"```  
* tree:  
    > "A recursive directory listing command or program that produces a depth-indented listing of files. It is available in Unix and Unix-like systems" - *[tree @ wiki](https://en.wikipedia.org/wiki/Tree_(command))*
    
    ```$ brew install tree```  
* fzf:  
    > "Interactive Unix filter for command-line that can be used with any list; files, command history, processes, hostnames, bookmarks, git commits, etc." - *[fzf](https://github.com/junegunn/fzf)*

    ```$ brew install fzf```
* vim:  
    > "Vim is a highly configurable text editor for efficiently creating and changing any kind of text. It is included as "vi" with most UNIX systems and with Apple OS X." - *[vim](https://www.vim.org/)*

    ```$ brew install vim```
* git:  
    > "Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency." - *[git](https://git-scm.com/)*

    ```$ brew install git```  
* python   
    > "Python is an interpreted, high-level, general-purpose programming language. Created by Guido van Rossum and first released in 1991, Python's design philosophy emphasizes code readability with its notable use of significant whitespace." - *[python](https://www.python.org/)*
    * python3:  
    ```$ brew install python```  
    * python2:  
    ```$ brew install python2```
* nvm:  
    > "Node Version Manager - POSIX-compliant bash script to manage multiple active node.js versions" - *[NVM](https://github.com/nvm-sh/nvm)*

    ```$ curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash```
* nodejs:  
    > "Node.js® is a JavaScript runtime built on Chrome's V8 JavaScript engine." - *[NodeJS](https://nodejs.org)*
    
    ```$ nvm install node```
* go:  
    > "Go is an open source programming language that makes it easy to build simple, reliable, and efficient software." - *[Go Lang](https://golang.org/)*
    
    ```$ brew install go```
* docker:  
    > "The Docker Platform is a set of integrated technologies and solutions for building, sharing and running container-based applications, from the developer’s desktop to the cloud." - *[Docker](https://www.docker.com)*

    ```$ brew cask install docker```
* vscode:  
    > "Visual Studio Code is a lightweight but powerful source code editor which runs on your desktop and is available for Windows, macOS and Linux. It comes with built-in support for JavaScript, TypeScript and Node.js and has a rich ecosystem of extensions for other languages (such as C++, C#, Java, Python, PHP, Go) and runtimes (such as .NET and Unity)." - *[Visual Studio Code](https://code.visualstudio.com/)*

    ```$ brew cask install visual-studio-code```