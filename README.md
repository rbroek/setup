# macOS setup

## Prerequisites

### [TextMate](https://macromates.com/)

### [iTerm2](https://www.iterm2.com/) with [Solarized](https://ethanschoonover.com/solarized/), [Powerline Shell](https://github.com/b-ryan/powerline-shell) and [Meslo Powerline Font](https://github.com/powerline/fonts/blob/master/Meslo%20Slashed/Meslo%20LG%20M%20Regular%20for%20Powerline.ttf)

* `Profiles` -> `Advanced` -> `Semantic History` -> `Open with editor...` -> `TextMate`

### [Xcode](https://itunes.apple.com/nl/app/xcode/id497799835?l=en&mt=12)

Install command line tools:
```
xcode-select --install
```

### [Homebrew](https://brew.sh/)

### ZSH
```
brew install zsh zsh-completions
chsh -s /bin/zsh
```

#### Install [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

Enable plugins in `~/.zshrc`:

```
plugins=(
  git
  bundler
  dotenv
  osx
  xcode
  php
  symfony
  symfony2
  brew
)
```

## dotfiles

### .gitconfig

```
[alias]
	lg = log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit
	ba = branch -a
	baf = branch -a --list "feature/*"
	rh = reset --hard HEAD
	cam = commit -am
	pr = pull --rebase
	fp = fetch --prune
	ftp = fetch --tags --prune
[user]
	name = <me>
	email = <email>
```

Or execute lines below to add `[user]` part:

```
git config --global user.name <me>
git config --global user.email <email>
```
