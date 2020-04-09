# New-Macbook
Setup scripts and links for web development on a new mac.


### Homebrew

```bash
/bin/bash -c “$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

### Iterm 2

```bash
brew cask install iterm2
```

#### Shell integration

You can enable better integration between your shell and iTerm2.
```
iTerm2 > Install Shell Integration
```

Then, add the following to your .zshrc: source ~/.iterm2_shell_integration.zsh.

### Git

```bash
brew install git
```

### Zsh

``` bash
brew install zsh
```

#### Update default shell

1. ```bash sudo vim /etc/shells ```
1. Add new line: ``` /usr/local/bin/zsh ```
1. Run ``` chsh -s /usr/local/bin/zsh ```
1. Restart the terminal and run ```bash echo $SHELL ``` and confirm it is zsh

#### Installing OhMyZsh

```bash
sh -c “$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

```bash
brew install romkatv/powerlevel10k/powerlevel10k
```

* Add the following to __.zshrc__ file:
 * ``` source /usr/local/opt/powerlevel10k/powerlevel10k.zsh-theme ```
 
**ZSH syntx hightlighting**
```bash
brew install zsh-syntax-highlighting
```

### NVM

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
```

```
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
```

> Restart the terminal and type ``` command -v nvm ``` to confirm it is installed

### Node JS

```bash
nvm install node  #install latest version
```

```bash
nvm install 6.14.4 # or 10.10.0, 8.9.1, etc
```

### Docker

```bash
brew cask install docker
```

### tldr

```bash
brew install tldr
```

### VSCode

```bash
brew cask install visual-studio-code
```


