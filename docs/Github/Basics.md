---
title: Basic Git Commands
parent: Using Github
nav_order: 2 
---

To use git, you will need to know how to clone a repository, pull changes from a remote repository to your local repository, push changes from your local repository to a remote repository, and how to change branches.

Besides `git clone`, all other git commands should be executed in the root directory of a repository.

### Table of Contents
{: .no_toc}

1. Cloning a Repository
{:toc}

# Cloning a Repository

See [Cloning a repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository#cloning-a-repository) from the official docs.

```sh
git clone <The GitHub Repository HTTPS Link>
```

Example: Clone the [Sally-Electrical-Design](https://github.com/UAlberta-EcoCar/Sally-Electrical-Design) repository.

```sh
git clone https://github.com/UAlberta-EcoCar/Sally-Electrical-Design.git
```

## Cloning a Repository containing Git Submodules
If a repository has a `.gitmodules` file, then it has Git Submodules in it. 
After cloning a repository, execute the following command:

```sh
git submodule update --init --recursive
```

Alternatively, if you have not cloned the repository yet, add the `--recursive` flag to your `git clone` command to automatically clone any git submodules too.
```sh
git clone --recursive <The GitHub Repository HTTPS Link>
```

## Cloning a Branch

By default, cloning a repository will download every branch of that repository. To clone a specific branch of a repository add these parameters to your git clone command.

```sh
git clone -b <Branch Name> <The GitHub Repository HTTPS Link>
```

Example: Clone the [Relay-Board](https://github.com/UAlberta-EcoCar/Sally-Electrical-Design/tree/Relay-Board) branch of the [Sally-Electrical-Design](https://github.com/UAlberta-EcoCar/Sally-Electrical-Design) repository

```sh
git clone -b Relay-Board https://github.com/UAlberta-EcoCar/Sally-Electrical-Design.git
```

# Pulling Changes from a Repository

To pull changes from a remote repository use
```sh
git pull
```

To pull new branches and remove deleted branches use
```sh
git fetch --prune
```

# Pushing Changes to a Repository

Once you have made your changes it is time to push those changes to the remote repository. There are 3 steps to this.

1. Stage all your changes
    ```sh
    git add .
    ```

1. Commit your changes
    ```sh
    git commit -m "Your commit message"
    ```
    Commit messages should be a concise description of the changes made. Commit messages are written using [Imperative Mood](https://chris.beams.io/git-commit#imperative) and do not include periods. 

    Git commit messages have a well standardized format in the industry, for a more detailed guide check out [The seven rules of a great Git commit message](https://chris.beams.io/git-commit#seven-rules)

    Examples of commit messages:
    * Fix protocol error
    * Add search bar to header menu
    * Delete bad.txt
    * Format files

1. Push your changes
    ```sh
    git push
    ```

# Git Branches

## Changing Branches

Before switching branches, make sure to commit or stash the changes you made. To change branches use

```sh
git checkout <branch name>
```

If git cannot find the branch, then you may need to pull new branches from the remote repository. 

```sh
git fetch origin
```

## Creating a New Branch

To create a new Git branch, run the command

```sh
git checkout -b <new branch name>
```
