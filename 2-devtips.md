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

# Scientific Python development tips and tricks

## Code navigation

Learn how to speed up how you navigate through code.

### [Sidebar search]()

Now with more Regex!

### [Multi-line editing](https://code.visualstudio.com/docs/editor/codebasics#_multiple-selections-multicursor)

![](https://code.visualstudio.com/assets/docs/editor/codebasics/multicursor.gif)

### [IntelliSense](https://code.visualstudio.com/docs/editor/intellisense)

Have you ever been typing and a popup with an auto-completion or hint pop up in a menu that you could pick from?
[IntelliSense](https://code.visualstudio.com/docs/editor/intellisense) is a general term for a whole catagory of features like this including: code completion, parameter info, quick info, and member lists.
In VS Code it will automatically pop up as you type for [supported languages](https://code.visualstudio.com/docs/editor/intellisense#_intellisense-for-your-programming-language) or with `Ctrl+Space` | `Cmd+Space`.
If you are not sure what the little icons next to certian suggestions mean, you can see a [legend](https://code.visualstudio.com/docs/editor/intellisense#_types-of-completions) in the docs.

![](https://code.visualstudio.com/assets/docs/editor/intellisense/intellisense_docs.gif)

```{tip}
There are a lot of customization options for how and when for Intellesense popups to open, check them out here and tweak or even turn off to your hearts content ❤️
```

IntelliSense is not AI generated, it uses language servers and other fancy diagnostic tools to constantly be analyzing your code to make suggestions.
If you want to try writing code with AI suggestions as well, you can check out [GitHub Copilot](https://code.visualstudio.com/docs/editor/intellisense#_enhance-completions-with-ai) which we will cover TODO.

```{admonition} Exercise
Try typing some new code in the sample notebook [here](TODO) and see what IntelliSense suggests!
```

### [Symbol search](https://code.visualstudio.com/Docs/editor/editingevolved#_open-symbol-by-name)

### [Go To ...](https://code.visualstudio.com/Docs/editor/editingevolved#_go-to-type-definition)

### [Refactoring](https://code.visualstudio.com/docs/editor/refactoring)

![](https://code.visualstudio.com/assets/docs/editor/refactoring/rename.png)

### Snippets

### Keyboard shortcuts

### Bring your keymaps: vim/emacs/sublime/…


## Running and testing code

Now that we finally know our way around the editor it’s time to write and test some code! Here we’ll go through a few exercises that let you test the code you’ve written in the previous exercise and debug it.

### Running in scripts
- Play button with 

### [Tests extension](https://marketplace.visualstudio.com/items?itemName=LittleFoxTeam.vscode-python-test-adapter)

### Debugger

## Git and version control

You’ve written some code - it’s time to push it upstream. We’ll go over some exercises that let you use the built-in Git tools to interact with the repository we cloned in the previous section.

### Git integration: branching, staging, committing, diff in-line

### Git Lens + integration with Git

### Pre-commit hooks

### GitHub actions (extensions to run them locally)

### [Gitignore extension](https://marketplace.visualstudio.com/items?itemName=codezombiech.gitignore)

## Documentation

Don't forget to document your work! Here we'll go over some tools in VS Code and GitHub to level up your docs.

### Sphinx + readthedocs

### LaTeX math rendering extension

### Docusaurus + github pages

## Data science tools

After writing your code, let’s put it to use. Here we’ll cover some of VS Code’s specialized features for data science, and install some typical extensions that plug into the scientific Python ecosystem.

### Figures

### Jupyter notebooks: coding, testing and debugging

### Data wrangler

### Database queries
