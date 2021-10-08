# lchip-arch-repo

**`lchip-arch-repo`** is my custom third-party repository for Arch Linux. 

In the event my packages are removed from the [Arch User Repository](https://aur.archlinux.org/), and/or my software is not on the AUR because it does not meet the community's criteria for [rules of submission](https://wiki.archlinux.org/title/AUR_submission_guidelines#Rules_of_submission), one is able to easily download/install my packages with pacman after adding my repository.

##  How to install lchip-arch-repo

To add a 3rd party repository:

1) Add the following lines to the *very end* of `/etc/pacman.conf`:

```bash
[lchip-arch-repo]
SigLevel = Optional DatabaseOptional
Server = https://github.com/Lawrence-Chiappelli/$repo/blob/main/$arch/lchip-arch-repo.db?raw=true
```

2) Then, sync your repositories:

`$ sudo pacman -Sy`

3) Finally, install one of my packages with pacman. For example:

`$ sudo pacman -S screendimmer`

Where screendimmer is one of the package names listed below.

## List of packages currently in this repository
- `screendimmer` - ( [GitHub](https://github.com/Lawrence-Chiappelli/screendimmer) | [AUR](https://aur.archlinux.org/packages/screendimmer/) )

## Other

Special thanks to DistroTube for providing instructions on adding your own 3rd party repository and making the process straightforward.
