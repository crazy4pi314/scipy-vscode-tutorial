# Meet your coding best friend: VS Code 💖 - A hands-on tutorial on how to get the most out of the world’s most popular Python editor

This repository accompanies the [VS Code tutorial at SciPy 2023](https://cfp.scipy.org/2023/talk/RKV3PZ/) of the same title.

## Installation instructions

### Start instantly with GitHub Codespaces

1. Click on the green _Code_ button, and then on the _Codespaces_ tab to create a codespace.  

You should now have a VS Code window in your browser with the repository open, running in a Codespace (2 cores by default).

### Work on your computer

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