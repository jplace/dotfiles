# jplace's dotfiles

I use [chezmoi](https://chezmoi.io) to manage my dot files.

## Installing dotfiles

1. Install chezmoi using a package manager.

2. Initialize chezmoi with a path to this repository.

```bash
chezmoi init https://github.com/jplace/dotfiles.git
```

3. Use chezmoi to change the dotfiles.

```bash
chezmoi diff # show what changes chezmoi will make to my home directory
chezmoi apply -v # apply changes to my home directory
chezmoi edit ~/.zshrc # edit a file in chezmoi
chezmoi update -v # pull and apply latest changes from remote repository
```

4. Customize certain computers.
   * Change your _.gitconfig_ to use your work email address.

## Changing files

Change files using chezmoi and then apply them to your machine and commit them in git.

```bash
chezmoi edit ~/.zshrc
chezmoi diff
chezmoi apply
chezmoi cd
git commit -a -m "Update dotfiles"
git push
```
