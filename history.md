---
marp: true
---

# Erich Gamma

![gamma](static/history/gamma.jpg)

- Swiss computer scientist
- Co-author of "Design Patterns: Elements of Reusable Object-Oriented Software"
- Co-wrote JUnit software testing framework (which helped kickstart test-driven development)
- Lead designer of the Eclipse platform's Java Development Tools (JDT)
- 2011: How far can we push coding in the browser?

---

# [Monaco Editor](https://microsoft.github.io/monaco-editor/)
- Lightweight code editor running in the browser
- Used by OneDrive, Internet Explorer F12 tools
- Some thousands of users, but developers & platform not ready yet
- 2014: Pivot to desktop via node webkit => VS Code

---

# Visual Studio Code

- First Microsoft tool to run on Linux
- extensions talk to the main process via remote procedure calls

- 2015: release



---

# VS Code - technology
- Written in TypeScript (started around the same time)
- Ships to Windows, Linux, macOS as Electron app (built on top of Chromium and Node.js)
- Only uses standard web APIs, no web frameworks (React, Vue.js, ...)
- Language server protocol (LSP) for language support
  - talks only about documents and position
  - people came and implemented language servers for all kinds of languages

---

# VS Code - license
- MIT license
- Distribution adds Microsoft branding, turns on telemetry by default, access to extensions marketplace hosted by Microsoft (some extensions closed source)
- Alternative builds
    - [VSCodium](https://github.com/VSCodium/vscodium#why): desktop build without Microsoft branding, telemetry and marketplace
    open-vsx.org marketplace
    - [code-server](https://github.com/coder/code-server): VS Code in the browser (built by coder.com)
    - [OpenVSCode-server](https://github.com/gitpod-io/openvscode-server): VS Code in the browser (built by Gitpod)

---

# VS Code - the open source project
- \>10 years of development, >1M lines of code
- 2022: #1 repo on GitHub by number of contributors ([state of the octoverse](https://octoverse.github.com/2022/state-of-open-source))
- thousands of issues opened every month
  goal: reply within 24 hours
- monthly release cycle
  - week 1: debt, plan
  - week 2-3: run
  - week 4: end game
  - ship


- team: 35 

---

# Recent developments
- Native file system APIs in browsers allow Progressive Web Apps (PWAs) to access the file system
- VS Code = WASI runtime => vscode.dev extensions can run Python in the browser (including debugger)

---