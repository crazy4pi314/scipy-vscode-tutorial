# ![Raccon mascot bit in a header image working on a laptop with the title: Meet your coding best friend: VS Code💖](image.png)

## _A hands-on tutorial on how to get the most out of the world’s most popular Python editor_ presented at [SciPy 2023](https://cfp.scipy.org/2023/talk/RKV3PZ/).

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/crazy4pi314/scipy-vscode-tutorial?quickstart=1)

Visual Studio Code (VS Code) is a free code editor that runs on Windows, Linux, macOS and in your browser. This tutorial aims at Python programmers of all levels who are already using VS Code or are interested in doing so, and will take them from zero (installing VS Code) to a production setup for Python development. We will cover starter topics, such as customizing the UI and extensions, using code autocomplete, code navigation, debugging, and Jupyter Notebooks. We will also go into advanced use cases, such as remote development, pair programming via Live Share, Dev containers, GitHub Codespaces & more.

## Installation instructions

### Option 1: Start instantly in your browser with GitHub Codespaces

1. [Create a free GitHub account](https://github.com/join) if you don't have one already

1. On the landing page of [this repository](https://github.com/crazy4pi314/scipy-vscode-tutorial), click on the green _Code_ button, and then on the _Codespaces_ tab to create a codespace.

After a short while you should have a VS Code window in your browser with the repository open.

Note: by default, the container running your code space will have 2 CPU cores, 4 GB of RAM, and 32 GB of local storage.

### Option 2: Work on your computer

1. [Install VS Code](https://code.visualstudio.com/download)
1. [Install git](https://github.com/git-guides/install-git)
1. [Install Docker](https://docs.docker.com/engine/install/)
1. Clone this repository:  `git clone https://github.com/crazy4pi314/scipy-vscode-tutorial`
1. Open the repository in VS Code `code scipy-vscode-tutorial`

You should now have the repository open in your local VS Code instance.

## Tutorial outline

With VS Code ready to go, it's time to jump into the [tutorial outline](outline.md).


## Structure of this repository

This repository contains a [Dev Container](https://containers.dev/) setup that provides [conda](https://github.com/conda/conda) and [mamba](https://github.com/mamba-org/mamba) for setting up Python environments.
This repo contains a sample Conda environment file ([environment.yml](environment.yml)), demo Jupyter notebook, and Dev Container configuration files that describe how a containerized development can be built for the repo.
These configuration files work for both local Dev Containers as well as [Codespaces](https://github.com/features/codespaces), a GitHub-hosted cloud environment.

The Docker setup for the Dev Container starts with a miniconda image that then will install whatever conda environment file you have at the root of the repo.
There are some additional configuration options in the comments of the [Docker](.devcontainer/Dockerfile) and [devcontainer.json](.devcontainer/devcontainer.json) that have some examples of other steps you may want to add to your Dev Container, like what VS Code extensions to install when the container is launched.