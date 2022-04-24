<h1 align="center">Welcome to XotoMachine Dot Files! 👋</h1>

### TABLE OF CONTENTS

- [TABLE OF CONTENTS](#table-of-contents)
- [DIRECTORY](#directory)
- [INSTRUCTIONS NIM](#instructions-nim)
- [Setup tmux](#setup-tmux)
- [GIT SUBMODULES CHEATSHEET](#git-submodules-cheatsheet)

### DIRECTORY

- [INSTRUCTIONS STOW](./documentation/STOW.md)
- [INSTRUCTIONS NVIM](./nvim/README.md)
- [INSTRUCTIONS ZSH](./zsh/README.md)

### INSTRUCTIONS NIM

```shell
# BACKUP 
mv ~/.config ~/.config-BK
# CLONE
git clone --recurse-submodules https://github.com/xotomachine/xotomachine-dotfiles.git ~/.config > /dev/null
```

<hr>

### Setup tmux
```shell
# run tmux
tmux 
# prefix+space i to install all deps 
```

### GIT SUBMODULES CHEATSHEET

```shell
# HOW TO CREATE A SUBMODULE ?
git submodule add git@github.com:my_account/my_submodule.git path_to_my_submodule 

# INITALIZING THE LOCAL GIT CONFIGURATION WITH THE SUBMODULES LIST
git submodule init 

# UPDATE YOUR SUBMODULES (LAST VERSION)
git submodule update --remote 

# UPDATE AND INITIALIZE IF THE SUBMODULE IS NOT INITIALIZED.
# (1) INITIALIZE THE GIT CONFIGURATION WITH THE SUBMODULES LIST RETRIEVED FROM THE .GITMODULE FILE
# (2) CLONE THE SUBMODULE REPOSITORY
git submodule update --init

# IF YOU HAVE A SUBMODULE WITHIN A SUBMODULE, YOU WILL WANT TO USE
git submodule update --init --recursive 
```