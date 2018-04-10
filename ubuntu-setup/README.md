# ubuntu-setup
Procedures and files to re-create Ubuntu environment from scratch.

## bootstrap access to github, then clone this repository
```
ssh-keygen -t rsa -b 4096 -C "wayne@warrenfamilyhome.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
xclip -sel clip < ~/.ssh/id_rsa.pub
# in browser, from githum.com settings, paste SSH key
ssh -T git@github.com
```

## to update this repository
Run `make` to collect all the most recent configuration files.

Copy `vimrc.local` to `~/.vimrc` or `/etc/vim`. Copy `.tmux.conf` to `~/.tmux.conf`.
Copy .gitconfig to ~/.gitconfig. Create ~/bin and copy pathlist to ~/bin.

Add `.bashrc-WLW` to the end of `~/.bashrc`.
.
