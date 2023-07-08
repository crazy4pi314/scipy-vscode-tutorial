---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# The basics of Python development in VS Code

**Getting started** -  a brief overview of VS Code and how to install it.

- VS Code is the most popular IDE today. Why?
- Launching VS Code
- Browser (default)
- Local (Desktop icon / `code .`)

**An anatomy of the VS Code UI** - how to navigate VS Code’s user interface.

- Command Palette / Command center
- Activity bar
  - Open folder
  - Search
  - Help: `?`
- Status bar
- Accessibility (color themes, screen readers, screencast mode, etc.)
- VS Code terminal (xtermjs)
- [Navigating without a mouse](https://www.youtube.com/watch?v=dJWJ0hCAkAI)

**Exercise**: clone a repo from GitHub and open in Codespaces (or your preferred platform). We will be working with it for the rest of the tutorial. E.g.: numpy (Python + C extensions, could be interesting for debugging), matplotlib, scipy.

**Setting up your Python project** - We will set up an existing Python project and install the necessary extensions. This piece is fairy quick and self-guided.

- Extensions marketplace
- Find and install Python extension
- Environment management

**Exercise**: Create a new virtual environment, install a package with the env create command pallet or the built-in terminal. Then create a new Jupyter notebook or script and import the package.

- Python extension settings: formatters / linters
  - available as extensions: pylint, flake8, black, autopep8, ...

**Customize your ride** - setting up our environment for Python development

- Customizing Telemetry
- Color themes: Dark, Colorblind
- Auto save
- Settings sync
- Profiles
- Files default language

