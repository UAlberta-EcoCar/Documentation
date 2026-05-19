---
title: Using Github
nav_order: 2 
---

# Introducing Git

[Git](https://git-scm.com/) is a version control software used to track changes in files and folders. [GitHub](https://github.com/home) is the web platoform we use to host Git repositories. Think of it like a powered up Google Drive. There are lots of good online Git tutorials on youtube, so check them out if you want to dive deeper into Git. There is also the [official documentation](https://docs.github.com/en/get-started/using-git/about-git) on Github. This documentation will only focus on the basics, then some development practices. 

To get started with using Github, you will first need to create a Github account. Then set up Git on your computer. 

### Git Introduction in 100 Seconds
<iframe width="620" height="315"
  src="https://www.youtube.com/embed/hwP7WQkmECE"
  title="Git Explained in 100 Seconds "
  frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowfullscreen>
</iframe>

# File Organization in GitHub

How files are organized in Github will vary between organizations. At EcoCar, each car has its own GitHub repository (example: [Sally](https://github.com/UAlberta-EcoCar/Sally-Electrical-Design)). 
Git branches in these repositories will usually contain both the firmware and hardware for a single PCB (examples: [Relay-Board](https://github.com/UAlberta-EcoCar/Sally-Electrical-Design/tree/Relay-Board), [H2-Sensor-Board](https://github.com/UAlberta-EcoCar/Sally-Electrical-Design/tree/H2-Sensor-Board), etc). There is also an embedded C library, [EcoLib](https://github.com/UAlberta-EcoCar/EcoLib), that contains various drivers and functions used in embedded projects.
