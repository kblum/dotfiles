# Dot Files

Dot Files for Mac OS X.

Forked from [Ryan Bates Dot File](https://github.com/ryanb/dotfiles).

Uses [Oh My ZSH](https://github.com/robbyrussell/oh-my-zsh).


## Installation

You should have [Homebrew](http://brew.sh) installed. Homebrew can be installed as follows:

```terminal
ruby -e "$(curl -fsSL https://raw.github.com/mxcl/homebrew/go)"
```

Run the following commands in your terminal. It will prompt you before it does anything destructive.

```terminal
git clone git://github.com/kblum/dotfiles ~/.dotfiles
cd ~/.dotfiles
rake install
```

After installing, open a new terminal window to see the effects.

Feel free to customize the .zshrc file to match your preference.


## Features

If you're using git, you'll notice the current branch name shows up in the prompt while in a git repository.

There are several features enabled in Ruby's irb including history and completion. Many convenience methods are added as well such as "ri" which can be used to get inline documentation in IRB. See irbrc file for details.


## Uninstall

To remove the dotfile configs, run the following commands. Be certain to double check the contents of the files before removing so you don't lose custom settings.

```
unlink ~/.bin
unlink ~/.gitignore
unlink ~/.gemrc
unlink ~/.gvimrc
unlink ~/.irbrc
unlink ~/.vim
unlink ~/.vimrc
unlink ~/.zshrc # careful here
rm ~/.gitconfig
rm -rf ~/.dotfiles
rm -rf ~/.oh-my-zsh
chsh -s /bin/bash # change back to Bash if you want
```

Then open a new terminal window to see the effects.
