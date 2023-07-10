# Meet your coding best friend: VS Code💖
![Raccon mascot bit in a header image working on a laptop with the title: Meet your coding best friend: VS Code💖](static/image.png)

_A hands-on tutorial on how to get the most out of the world’s most popular Python editor_ 

> Tutorial for [SciPy 2023](https://cfp.scipy.org/2023/talk/RKV3PZ/), 2023-07-10, 13:30–17:30 (America/Chicago), Classroom 103.

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/crazy4pi314/scipy-vscode-tutorial?quickstart=1)

Visual Studio Code (VS Code) is a free code editor that runs on Windows, Linux, macOS and in your browser. This tutorial aims at Python programmers of all levels who are already using VS Code or are interested in doing so, and will take them from zero (installing VS Code) to a production setup for Python development. We will cover starter topics, such as customizing the UI and extensions, using code autocomplete, code navigation, debugging, and Jupyter Notebooks. We will also go into advanced use cases, such as remote development, pair programming via Live Share, Dev containers, GitHub Codespaces & more.

## Tutorial schedule

We end each section with a recap to go over everything we’ve covered and an opportunity to ask questions.

| Time  | Duration | Topic                  |
|-------|----------|------------------------|
| 13:30 | 50 min   | [The basics of Python development in VS Code](1-basics.md)        |
| 14:20 | 10 min   | Break                  |
| 14:30 | 50 min   | [Scientific Python development tips and tricks](2-devtips.md)       |
| 15:20 | 10 min   | Break                  |
| 15:30 | 50 min   | [Interacting with remote resources](3-remote.md)        |
| 16:20 | 10 min   | Break                  |
| 16:30 | 50 min   | [Working together, but make it fast](4-collaboration.md) |
| 17:20 | 10 min   | Closing remarks        |
## Setup Instructions

### **Option 1:** Work on your computer

1. [Install VS Code](https://code.visualstudio.com/download)
2. Install local development environment

  - Variant A: Native installation
    - [Install Git](https://github.com/git-guides/install-git)
    - [Install Miniconda](https://docs.conda.io/en/latest/miniconda.html)
    - Note for Windows users: You may want to [install WSL2](https://learn.microsoft.com/en-us/windows/wsl/install) and install Git and Miniconda in the Linux subsystem.
  - Variant B: Use Linux containers. Just [install Docker](https://docs.docker.com/engine/install/)

3. Clone this repository:  `git clone https://github.com/crazy4pi314/scipy-vscode-tutorial`
4. Open the repository in VS Code `code scipy-vscode-tutorial`
5. (Docker only) With your repo open in VS Code, install the [Development Container](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension (if you don't already have it) which will give you command pallet options to re-open the repo in a dev container.

You should now have the repository open in your local VS Code instance.

### **Option 2:** Start instantly in your browser with GitHub Codespaces

1. [Create a free GitHub account](https://github.com/join) if you don't have one already

1. On the landing page of [this repository](https://github.com/crazy4pi314/scipy-vscode-tutorial), click on the green _Code_ button, and then on the _Codespaces_ tab to create a codespace.

After a short while you should have a VS Code window in your browser with the repository open.

This option gives you a fully functional VS Code environment (with [some limitations](https://code.visualstudio.com/docs/remote/codespaces#_known-limitations-and-adaptations)), and should work on laptops and tablets alike.

> Note: GitHub codespaces come with [120 core-hours and 15 GB-months for free](https://docs.github.com/en/billing/managing-billing-for-github-codespaces/about-billing-for-github-codespaces) for all GitHub accounts (180 core-hours for verified student accounts).
By default, the container running your codespace will have 2 CPU cores, 4 GB of RAM, and 32 GB of local storage.

### **Option 3:** Follow along on vscode.dev

If neither option 1 nor 2 works for you, you can still shadow the presenters in a read-only [LiveShare](https://code.visualstudio.com/learn/collaboration/live-share) session in your web browser.
Contrary to option 2 this does not require a GitHub account - all you need is a web browser.

We will share a https://vscode.dev/liveshare link at the start of the session.
When opening the link, select "Continue on web" and "Continue as anonymous".


## Structure of this repository

This repository contains a [Dev Container](https://containers.dev/) setup that provides [conda](https://github.com/conda/conda) and [mamba](https://github.com/mamba-org/mamba) for setting up Python environments.
This repo contains a sample Conda environment file ([environment.yml](environment.yml)), demo Jupyter notebook, and Dev Container configuration files that describe how a containerized development can be built for the repo.
These configuration files work for both local Dev Containers as well as [Codespaces](https://github.com/features/codespaces), a GitHub-hosted cloud environment.

The Docker setup for the Dev Container starts with a miniconda image that then will install whatever conda environment file you have at the root of the repo.
There are some additional configuration options in the comments of the [Docker](.devcontainer/Dockerfile) and [devcontainer.json](.devcontainer/devcontainer.json) that have some examples of other steps you may want to add to your Dev Container, like what VS Code extensions to install when the container is launched.

## References

* [bees.csv](data/bees.csv): Diller, S.N., Schaeffer, J.S., Grundel, R., Pavlovic, N.B., McKenna, J.E. Jr., Esselman, P.C., 2020, Bee-Gap: Ecology, Life-History, and Distribution of Bee Species in the United States 2017: U.S. Geological Survey data release, https://doi.org/10.5066/P9QHQNNS.

## Contributors

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->
