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

## Example - VS Code Desktop application with Remote SSH extension
![VS Code architecture](static/architecture/architecture.png)
- Local VS Code client version of local client and remote server must match exactly

## Example - VS Code Desktop application with Remote SSH extension
![VS Code architecture](static/architecture/extensions.png)
---

![VS Code architecture](static/architecture/architecture.png)
- Local VS Code client version of local client and remote server must match exactly
- VS Code version of local client and remote server must match exactly

---

# VS Code - client/server architecture
![VS Code architecture](static/architecture/architecture.png)
- Local VS Code client version of local client and remote server must match exactly
- VS Code version of local client and remote server must match exactly

---

---


---

# Recent developments
- Native file system APIs in browsers allow Progressive Web Apps (PWAs) to access the file system
- VS Code = WASI runtime => vscode.dev extensions can run Python in the browser (including debugger)

---