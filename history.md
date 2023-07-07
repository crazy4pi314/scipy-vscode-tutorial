---
jupytext:
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.14.7
---

# Erich Gamma

- Born in Zurich, Switzerland
- Gang of four: Authors of the book "Design Patterns: Elements of Reusable Object-Oriented Software"
- Co-wrote JUnit software testing framework (common library for Java projects, helped create test-driven development)
- Lead designer of the Eclipse platform's Java Development Tools (JDT)
  - everything is a plugin
  - everything is loaded in one project
  - everything is written in Java
- Joined Microsoft Visual Studio team in 2011

+++

# Monaco
- How far can you get with JavaScript in the browser?
- First Microsoft tool to run on Linux
- extensions talk to the main process via remote procedure calls
- Developers and platform not yet ready => needed to go to the desktop (via electron)

+++

# Language server protocol
- talks only about documents and position
- people came and implemented language servers for all kinds of languages


+++

# VS Code - technology
- Written in TypeScript (started around the same time)
  - no `Any` variables
- Ships to Windows, Linux, mavOS as Electron app (built on top of Chromium and Node.js)
- Only uses standard web APIs, no web frameworks (React, Vue.js, ...)

+++

# VS Code - license
- MIT license
- Distribution adds Microsoft branding, turns on telemetry by default, access to extensions marketplace hosted by Microsoft (some extensions closed source)
- Alternative builds
    - [VSCodium](https://github.com/VSCodium/vscodium#why): desktop build without Microsoft branding, telemetry and marketplace
    - [code-server](https://github.com/coder/code-server): VS Code in the browser (built by coder.com)
    - [OpenVSCode-server](https://github.com/gitpod-io/openvscode-server): VS Code in the browser (built by Gitpod)

+++

# VS Code - the open source project
- >10 years of development, >1M lines of code
- 2022: #1 repo on GitHub by number of contributors ([state of the octoverse](https://octoverse.github.com/2022/state-of-open-source))
- thousands of issues opened every month
  goal: reply within 24 hours
- monthly release cycle
  - week 1: debt, plan
  - week 2-3: run
  - week 4: end game
  - ship


- team: 35 

+++

# Recent developments
- Native file system APIs in browsers allow Progressive Web Apps (PWAs) to access the file system
- VS Code = WASI runtime => vscode.dev extensions can run Python in the browser (including debugger)
