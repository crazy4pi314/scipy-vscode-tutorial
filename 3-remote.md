# Interacting with remote resources

## Interlude: some background

The modular design of VS Code lets you choose where to run the user interface and the backend independently. Let's understand how this came to be.

- [A brief history of VS Code](history.md)
- [VS Code's basic architecture](architecture.md)

## The Remote development extension pack
Developing inside pre-packaged local DevContainers, on a virtual machine in the cloud, in a GitHub Codespace, and more.

- [WSL](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl): Windows Subsystem for Linux was VS Code's first remote development scenario
- [Remote - SSH](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-ssh): Connect your local VS Code to a remote machine over SSH
  - Automatic port forwarding (web apps, Jupyter servers)
- [Remote - Tunnels](https://marketplace.visualstudio.com/items?itemName=ms-vscode.remote-server): Reach remote machines behind firewalls
- [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers): Work inside containers & make your environment reproducible for others
  - Look at the [`devcontainer.json`](.devcontainer/devcontainer.json) in this repository
  - [GitHub Codespaces](https://github.com/features/codespaces) = Dev Containers hosted by GitHub

**Exercise**
Pick a combo of local/host VS Code scenarios, and share with your group, involving them if you can

Here are some ideas:
- Package maintainers: Create a `devcontainer.json` for your repository & let your neighbor try out your package
- Start a GitHub codespace on the `scipy-vscode-tutorial` repository and connect to it from your local VS Code via tunnel
- Start a VS Code server for someone else and let them connect
- Windows: install WSL, and use [this trick](https://stackoverflow.com/questions/60150466/can-i-ssh-from-wsl-in-visual-studio-code/66048792#66048792) to have VS Code read your SSH config file from the WSL environment


## vscode.dev / github.dev
Everything runs inside your browser

- Press `.` on any GitHub repo
- LiveShare
- Python via [Python for the Web](https://code.visualstudio.com/docs/python/python-web)
- Code on your tablet
- [Continue working on](https://code.visualstudio.com/docs/editor/vscode-web#_continue-working-in-a-different-environment) a different device without having to commit


**Exercise**

Start a VS Code server on your machine and connect to it from your browser (same device, or tablet / phone / ...)