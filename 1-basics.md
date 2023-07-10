# The basics of Python development in VS Code

## Some facts & figures

- [Stack Overflow Annual Developer Surveys](https://insights.stackoverflow.com/survey): VS Code is the most popular integrated development environment (IDE) since 2018.

  | Year | VS Code* | Rank |
  |------|----------|------|
  | 2015 | Release  | -    |
  | 2016 | 7%       | 13   |
  | 2017 | 23%      | 5    |
  | 2018 | 35%      | 1    |
  | 2019 | 51%      | 1    |
  | 2020 | -        | -    |
  | 2021 | 71%      | 1    |
  | 2022 | 74%      | 1    |
  | 2023 | 74%      | 1    |

  *Percentage of respondents using VS Code as a developer environment (multiple answers possible).

- [2022 State of the Octoverse](https://octoverse.github.com/2022/state-of-open-source): [github.com/microsoft/vscode](https://github.com/microsoft/vscode) is `#1` repository on GitHub by number of contributors 
- The [VS Code Marketplace](https://marketplace.visualstudio.com/search?target=VSCode&category=All%20categories&sortBy=Installs) has 49k extensions as of July 2023

What brought _us_ to VS Code?

## Getting started

A brief overview of VS Code.

- Launching VS Code
  - Local (Desktop icon / `code .`)
  - Browser: Primary option for workshop (https://vscode.dev/, `.` on any GitHub page)

> **Prep exercise**: Follow the setup instructions in the [README](README.md#setup-instructions). For quick set-up we recommend using Codespaces directly from GitHub!

## An anatomy of the VS Code UI

How to navigate VS Code’s user interface.

- Command Palette / Command center
- Activity bar
  - Open folder
  - Search
  - Help: `?`
- Status bar
- Panel
- [Accessibility](https://code.visualstudio.com/docs/editor/accessibility) (color themes, screen readers, screencast mode, etc.)
- [VS Code terminal](https://code.visualstudio.com/docs/terminal/advanced) (xtermjs)
- [Navigating without a mouse](https://www.youtube.com/watch?v=dJWJ0hCAkAI)

> **Exercise**: Explore VS Code acessibility
>
> 1. Browse to the tutorial repo on GitHub and try opening it either in your browser (press `.` when on repo page) or cloning it locally and opening with `code .`.
> 2. Use the Command Palette to Zoom in and Zoom out (editor and/or view).
> 3. Search for Color Themes using the Extensions tab. You can find extensions or color themes that are accessible for color vision deficiencies, for example, take a look at the color blind-friendly extensions. If you are using a [screen reader](https://code.visualstudio.com/docs/editor/accessibility#_screen-readers) such as NVDA, JAWS and VoiceOver, try using it with VS Code!
> 4. Use the Command Palette or "gear" icon to change your Color Theme to a non-default one.
>

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
> 1. Create a new profile or use one of the templates.
> 2. Either in your local or browser-based VS Code, try customizing some settings, themes, font sizes, etc.
> 3. Export your current profile as a gist (or locally if you prefer).
> 4. Copy-paste the URL for your profile gist, and add it to the [discussion page](https://github.com/crazy4pi314/scipy-vscode-tutorial/discussions/17).
> 5. Try making a profile for presenting/screencasting or maybe a distraction-free writing space and take turns sharing all your cool new profiles with your team 😄
> 6. Try importing a profile created by someone else via the `Profiles` > `Import Profile...` option in the Gear menu! You can find @crazy4pi314's profiles [here](https://gist.github.com/crazy4pi314/a3b1157dcd0873d471fb79cf5dffaba4).
>

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
> 1. In the Codespace for this workshop or locally (in a Dev Container) on your machine, create a new virtual environment by running:
>
> ```bash
> cd scipy-vscode-tutorial
> conda install -n base -conda-forge mamba
> mamba env create -f environment.yml
> ```
>
> 2. Install the tutorial package by running:
>
> ```bash
> pip install -e .
> ```
>
> 3. Use the Command Palette to run the `Python: Select Interpreter` command and set it to the `tutorial` environment you just created.
> 4. Use the Command Palette to create a new Interactive Window using the `Jupyter: Create Interactive Window` command.
> 5. Run the following lines to test your environment:
>
>   ```python
>   from tutorial import welcome
>   welcome()
>   ```
>
