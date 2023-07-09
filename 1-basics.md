# The basics of Python development in VS Code

## Getting started

A brief overview of VS Code and how to install it.

- VS Code is the most popular IDE today. Why?
- Launching VS Code
  - Local (Desktop icon / `code .`)
  - Browser: Primary option for workshop (https://vscode.dev/, `.` on any GitHub page)

## An anatomy of the VS Code UI

How to navigate VS Code’s user interface.

- Command Palette / Command center
- Activity bar
  - Open folder
  - Search
  - Help: `?`
- Status bar
- [Accessibility](https://code.visualstudio.com/docs/editor/accessibility) (color themes, screen readers, screencast mode, etc.)
- [VS Code terminal](https://code.visualstudio.com/docs/terminal/advanced) (xtermjs)
- [Navigating without a mouse](https://www.youtube.com/watch?v=dJWJ0hCAkAI)

> **Exercise**: Explore VS Code acessibility
>
> Find a repo on GitHub and try opening it either in your browser (press `.` when on repo page). Try navigating around the UI, and turn on some acessability settings and give them a go!

## Customize your UI

More fun and helpful UI features and settings.

- Some key settings to check:
  - [Customizing Telemetry](https://code.visualstudio.com/docs/getstarted/telemetry)
  - Color themes: Dark, Colorblind
  - [Auto save](https://code.visualstudio.com/docs/editor/codebasics#_save-auto-save)
  - [Files default language](https://code.visualstudio.com/docs/languages/overview)
- [Settings sync](https://code.visualstudio.com/docs/editor/settings-sync)
- [Profiles](https://code.visualstudio.com/docs/editor/profiles)
  - [Python Dev profile template](https://code.visualstudio.com/docs/editor/profiles#_python-profile-template)
  - [Data Science profile template](https://code.visualstudio.com/docs/editor/profiles#_data-science-profile-template)
  - [Sarah's profile collection](https://dev.to/crazy4pi314/profiles-for-fun-and-profit-how-to-use-profiles-to-customize-vs-code-57hj)
- [Extensions marketplace](https://code.visualstudio.com/docs/editor/extension-marketplace)
  - Don't see what you need? [Make your own!](https://code.visualstudio.com/api/get-started/your-first-extension)

> **Exercise**: Share your profile
>
> Either in your local or browser-based VS Code, try customizing some settings, themes, etc. either from a blank profile or one of the templates. Then export your current editor config as a gist (or locally if you prefer). If you have the URL for your profile gist, add it to the [discussion page](https://github.com/crazy4pi314/scipy-vscode-tutorial/discussions/17). 
> Try making a profile for presenting/screencasting or maybe a distraction-free writing space and take turns sharing all your cool new profiles with your team 😄

## Setting up for Python development

We will set up a Python project and install the necessary extensions. This piece is fairy quick and self-guided.

- [Python Environments in VS Code](https://code.visualstudio.com/docs/python/environments#_creating-environments)
  - Default intrepreter settings
  - [Python environment manager](https://marketplace.visualstudio.com/items?itemName=donjayamanne.python-environment-manager)
- Common Python extensions
  - [Python extension pack by Don Jayamanne](https://marketplace.visualstudio.com/items?itemName=donjayamanne.python-extension-pack)
  - [Jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)
  - formatters / linters: pylint, flake8, black, autopep8, ...

> **Exercise**: New Python project from scratch
>
> In the Codespace for this workshop or locally (in a Dev Container) on your machine, use VS Code to create a new virtual environment, install the `emoji` packages with the `Python: Create Environment` command from the command pallet or the built-in terminal. Check that you have the intrepreter setup correclty by opening a new Jupyter notebook or script and import the package(s):
>
> ```python
> import emoji
> print(emoji.emojize("Meet your coding best friend: VS Code :red_heart:"))
> ```

>
```
