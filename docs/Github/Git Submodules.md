---
title: Using Git Submodules
parent: Using Github
nav_order: 3 
---

Git submodules are Git repositories inside of other Git repositories. Most firmware at EcoCar uses the [EcoLib](https://github.com/UAlberta-EcoCar/EcoLib) embedded C library, which is added as a Git submodule. 

This guide will only cover cloning a Git repository containing Git Submodules and adding a Git Submodule to your repository. For a more detailed tutorial see the [Git Submodule Tutorial](https://www.geeksforgeeks.org/git/git-submodule/) at GeeksForGeeks[^1].

# Cloning a Repository containing Git Submodules

If a repository has a `.gitmodules` file, then it has Git Submodules in it. 
After cloning a repository, execute the following command:

```sh
git submodule update --init --recursive
```

Alternatively, if you have not cloned the repository yet, add the `--recursive` flag to your `git clone` command to automatically clone any git submodules too.

```sh
git clone --recursive <The GitHub Repository HTTPS Link>
```

# Adding a Git Submodule

In the root directory of your Git Repository execute the command

```sh
git submodule add <repository-url> <path>
```

Example: Add the [EcoLib](https://github.com/UAlberta-EcoCar/EcoLib)
repository to your git repository, add it to a folder with the path `MyFirmware/Libs/`

```sh
git submodule add https://github.com/UAlberta-EcoCar/EcoLib.git MyFirmware/Libs/
```

----

[^1]: [GeeksForGeeks Git Submodule Tutorial](https://www.geeksforgeeks.org/git/git-submodule/).
