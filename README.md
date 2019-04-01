# macOS setup

## Prerequisites
- [Homebrew](https://brew.sh/)
- 

### Install zsh
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

