# Interacting with remote resources

## Interlude: some background

The modular design of VS Code lets you choose where to run the user interface and the backend independently. Let's understand how this came to be.

- [A brief history of VS Code](history.md)
- [VS Code's extension architecture](architecture.md)

## The Remote development extension pack

Developing inside pre-packaged local DevContainers, on a virtual machine in the cloud, in a GitHub Codespace, and more.

- [WSL](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl): Windows Subsystem for Linux was VS Code's first remote development scenario
- [Remote - SSH](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-ssh): Connect your local VS Code to a remote machine over SSH
  - Automatic port forwarding (web apps, Jupyter servers)
- [Remote - Tunnels](https://marketplace.visualstudio.com/items?itemName=ms-vscode.remote-server): Reach remote machines behind firewalls
  - On remote machine, open a terminal and run:
    ```
    curl -Lk 'https://code.visualstudio.com/sha/download?build=stable&os=cli-alpine-x64' --output vscode_cli.tar.gz
    tar -xf vscode_cli.tar.gz
    ./code tunnel
    ```
  - Connect from Desktop app via `Remote Tunnels: Connect to tunnel`
- [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers): Work inside containers & make your environment reproducible for others
  - The [`devcontainer.json`](.devcontainer/devcontainer.json) in this repository follows the [Development Containers standard](https://containers.dev/)
  - [GitHub Codespaces](https://github.com/features/codespaces) = Dev Containers hosted by GitHub

**Exercise**
Play with different UI/backend scenarios, and share with your group, involving them if you can

Here are some ideas:

- Contribute a `devcontainer.json` to your favorite repository on GitHub & make it easier for everyone to give the package a try
- Connect remotely to a machine you typically use a command line editor like vim/emacs on
  - For tutorial participants: 
    - Connect to JupyterHub, choose user/password
    - Click New => Terminal
    - Create a file `.ssh/authorized_keys` and add your SSH public key to it
    - Connect to Hub using `jupyter-<username>` at port 2222
- Windows users: install WSL, and use [this trick](https://stackoverflow.com/questions/60150466/can-i-ssh-from-wsl-in-visual-studio-code/66048792#66048792) to have VS Code read your SSH config file from the WSL environment
- Start a GitHub codespace on the `scipy-vscode-tutorial` repository and connect to it from your local VS Code via "Open Codespace in new Window"
- Start a VS Code server (`code tunnel`) on your machine and connect from your tablet / let your neighbor connect

## vscode.dev / github.dev

Everything runs inside your browser

- Press `.` on any GitHub repo
- [Continue working on](https://code.visualstudio.com/docs/editor/vscode-web#_continue-working-in-a-different-environment) a different device without having to commit
- More "workspace extensions" are coming to vscode.dev
  - Already there: LiveShare, some language servers, ...

**Exercise**

- There are now 3 different ways to make a pull request to a GitHub repository using just your browser. What are they?
- Try the new [Python for the Web](https://code.visualstudio.com/docs/python/python-web) directly on [insiders.vscode.dev](https://insiders.vscode.dev/)
