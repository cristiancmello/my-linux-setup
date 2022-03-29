
# Set up ZSH with Powerline9k

```sh
sudo apt install \
    git \ 
    zsh \
    zsh-theme-powerlevel9k \ 
    zsh-syntax-highlighting

# Define ZSH as default shell
sudo usermod -s /usr/bin/zsh $(whoami)

# Install Oh-My-ZSH
sh -c "$(wget https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"

# Enable PowerLevel9k
echo "source /usr/share/powerlevel9k/powerlevel9k.zsh-theme" >> ~/.zshrc

# Enable Syntax Highlighting
echo "source /usr/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ~/.zshrc

exit
```

### Add Plugins

```sh
vim ~/.zshrc
```

* Search for `plugins` section

```zshrc
plugins=(
    git
    colored-man-pages
)
```