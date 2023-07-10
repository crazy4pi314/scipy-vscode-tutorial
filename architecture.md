## VS Code - client/server architecture
- Graphical user interface runs inside
  - Electron app: VS Code Desktop application
  - Browser: GitHub Codespace, vscode.dev, github.dev, ...
- Backend runs inside
  - Electron app: VS Code Desktop application
  - Local WSL: WSL extension
  - Remote computer: Remote SSH extension, Tunnel extension
  - Local container: Dev Containers extension
  - Container hosted by GitHub: GitHub Codespaces
  - Browser: vscode.dev, github.dev (limited functionality)

## Example - VS Code Desktop with Remote SSH extension
![VS Code architecture](static/architecture/architecture.png)
- VS Code version of local client and remote server must match exactly

## Overview - Where are the extensions running?
![Extension hosts](static/architecture/extensions.png)
