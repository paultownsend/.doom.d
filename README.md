# .doom.d

My private configuration for [Doom Emacs](https://github.com/hlissner/doom-emacs).

## Install

### Emacs

``` sh
brew tap d12frosted/emacs-plus
brew install emacs-plus@27
ln -s /usr/local/opt/emacs-plus@27/Emacs.app /Applications
```

### Doom

``` sh
brew install ripgrep fd
git clone --depth 1 https://github.com/hlissner/doom-emacs ~/.emacs.d
git clone https://github.com/paultownsend/.doom.d ~/.doom.d
~/.emacs.d/bin/doom install
```

#### :term vterm

``` sh
brew install cmake libvterm
```

#### :tools editorconfig

``` sh
brew install editorconfig
```

#### :lang python

Use `M-x lsp-install-server` and select `mspyls` as the server to install.

#### :email mu4e

``` sh
brew install mu
mbsync -a
mu init --maildir=~/Mail --my-address=...@... --my-address=...@...
touch ~/Mail/Spam/.noindex
mu index
```
