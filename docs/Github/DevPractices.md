---
title: Best Practices
parent: Using Github
nav_order: 5 
---

### Table of Contents
{: .no_toc}

1. The ReadMe File
{:toc}

# The ReadMe File

Taken from the GitHub docs[^1], 
a README is often the first item a visitor will see when visiting your repository. README files typically include information on:

* What the project does
* Why the project is useful
* How users can get started with the project
* Where users can get help with your project
* Who maintains and contributes to the project

All branches in a car's repository (ex: [Sally](https://github.com/UAlberta-EcoCar/Sally-Electrical-Design)) 
should already contain a `README.md` file. In Sally's repository, each branch will contain the PCB and firmware files for 
a single PCB. It is good practice for the README files of those branchs to include information on:

* What the board does
* How to contribute
  * What programs to install, third part dependencies, etc.
  * Any code formatters used.
  * If a git submodule is used, then it is a good idea to record the last working commit of the git submodule used. 

    If in the future, the git submodule is updated with a change that breaks functionality, you can immediately checkout the last working commit of the submodule.
    An example of recording this is in the FOC-Board's [repository](https://github.com/UAlberta-EcoCar/Sally-Electrical-Design/tree/FOC-Board#branch-for-the-original-foc-board)
* Authors

# The .gitignore File

You may want git to ignore certain files when commiting changes. That is where a `.gitignore` file comes in handy.
Examples of common files to ignore are build files, cache files, files containing sensitive information, files containing API keys, etc.

In a `.gitignore` file each line represents a pattern that you want to match to files that will be ignored. See the [official documentation](https://git-scm.com/docs/gitignore)[^2] for more information on pattern matching. 

Luckily there are `.gitignore` templates that already exist and can be 
added to your repository without any modifications. 
A collection of `.gitignore` templates can be found in the [gitignore repository](https://github.com/github/gitignore/tree/main).

There are 2 `.gitignore` templates that you will likely use:

1. For KiCad projects, there is a KiCad [.gitignore file](https://github.com/github/gitignore/blob/main/KiCad.gitignore)
  that should be copied into the root of your KiCad project.
1. For STM32 projects, there is a STM32 [.gitignore file](https://github.com/github/gitignore/blob/main/Global/STM32CubeIDE.gitignore)
  that should be copied into the root of your STM32 project.

# Versioning 

The industry wide standard to version software is to follow [Semantic Versioning](https://semver.org/) rules[^3].
Versioning is useful if you want to record a snapshot of your project for future reference.
Usually this will be done after your board and firmware are developed and eveything is working.
That way you can always access the last working version of your work.

In git, the way to create a new version is to create a [tag](https://git-scm.com/book/en/v2/Git-Basics-Tagging).
Git tags are like branches, except they are immutable. You cannot make changes to a tag.

Because the branches in a car's repository are each dedicated to a PCB, the name of the PCB should be part of the tag's name.
Here's a typical process for creating a tag in a car's repository.

```sh
# Create a new tag
git tag <Name of PCB>-<version>
# Push that tag to the remote repository
git push --tags
```

Example: Create version 1.0.0 of the [FOC-Board](https://github.com/UAlberta-EcoCar/Sally-Electrical-Design/tree/FOC-Board)
```sh
git tag FOC-Board-v1.0.0
git push --tags
```

# Troubleshooting Git

[Oh Shit, Git!?!](https://ohshitgit.com/)

----

[^1]: [GitHub README Documentation](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes).

[^2]: [.gitignore Documentation](https://git-scm.com/docs/gitignore)

[^3]: [Semantic Versioning](https://semver.org/)
