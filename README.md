# macOS setup

## Prerequisites

### [TextMate](https://macromates.com/)

### [iTerm2](https://www.iterm2.com/) with [Solarized](https://ethanschoonover.com/solarized/), [Powerline Shell](https://github.com/b-ryan/powerline-shell) and [Meslo Powerline Font](https://github.com/powerline/fonts/blob/master/Meslo%20Slashed/Meslo%20LG%20M%20Regular%20for%20Powerline.ttf)

* `Profiles` -> `Advanced` -> `Semantic History` -> `Open with editor...` -> `TextMate`

### [Xcode](https://itunes.apple.com/nl/app/xcode/id497799835?l=en&mt=12)
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

