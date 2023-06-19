# Tutorial outline

We will be using Live Share so instead of repeating the instructions on your VS Code instance, you can ualso join the VS Code session directly from your browser or local VS Code instance. Each section contains a set of self-guided exercises, some examples of which are highlighted in the outline below.

We end each section with a recap to go over everything we’ve covered and an opportunity to ask questions.

## The basics: VS Code editor and Python extension overview [1 hour]

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
- Status bar
- Accessibility (color themes, screen readers, screencast mode, etc.)
- VS Code terminal (xtermjs)

**Exercise**: clone a repo from GitHub and open in Codespaces (or your preferred platform). We will be working with it for the rest of the tutorial. E.g.: numpy (Python + C extensions, could be interesting for debugging), matplotlib, scipy.

**Setting up your Python project** - We will set up an existing Python project and install the necessary extensions. This piece is fairy quick and self-guided.

- Extensions marketplace
- Find and install Python extension
- Environment management

**Exercise**: Create a new virtual environment, install a package with the env create command pallet or the built-in terminal. Then create a new Jupyter notebook or script and import the package.

- Python extension settings: formatters / linters

**Customize your ride** - setting up our environment for Python development

- Customizing Telemetry controls
- Color themes
- Auto save
- Settings sync
- Profiles
- Files default language

## Break: 10 min

## Scientific Python development tips and tricks [1 hour]

**Code navigation** - Learn how to speed up how you navigate through code.

- IntelliSense
- Symbol search
- Multi-line editing
- Find references
- Regex search
- Code transform

**Running and testing code** - Now that we finally know our way around the editor it’s time to write and test some code! Here we’ll go through a few exercises that let you test the code you’ve written in the previous exercise and debug it.

- Shift + enter
- YAML extension
- Code runner extension
- Unit tests extension
- Debugger


**Git and version control** - You’ve written some code - it’s time to push it upstream. We’ll go over some exercises that let you use the built-in Git tools to interact with the repository we cloned in the previous section.

- Git integration: branching, staging, committing, diff in-line
- Git Lens + integration with Git
- Pre-commit hooks
- GitHub actions (extensions to run them locally)

**Documentation** - Don't forget to document your work! Here we'll go over some tools in VS Code and GitHub to level up your docs.

- Sphinx + readthedocs
- LaTeX math rendering extension
- Docusaurus + github pages

**Data science tools** - After writing your code, let’s put it to use. Here we’ll cover some of VS Code’s specialized features for data science, and install some typical extensions that plug into the scientific Python ecosystem.

- Figures
- Jupyter notebooks: coding, testing and debugging
- Data wrangler
- Database queries


## Break: 10 min


## Advanced development Part I: interacting with remote resources [45 minutes]

**Work where you want to** - Here we will go over some ways on how to work with VS Code on any device and how you can transfer your settings from your local editor. This can be helpful when on-the-go or if you want to make your project easily accessible without any installation requirements. We’ll cover basic tools you will need to develop on a remote resource, such as a cloud instance for compute-heavy workloads.

- Interlude: where does VS Code come from: Monaco, fully-fledged source-code editor for the browser
- GitHub Codespaces - Run Python in the browser
- Remote development extension pack
- SSH remote extension
- Automatic port forwarding
- (Optional) Setting up VS Code with WSL
- DevContainers
- Vscode.dev
- Jupyter servers
- Tunneling


**Home brewing** - Finally, if you prefer not to use cloud resources or have extra compute resources lying around, we’ll show you how you can use VS Code on your own server. We’ll also cover setting up VS Code iPad or Surface tablet, for developing on-the-go. If you’d like to set up the latter with us during the tutorial, make sure to bring your own tablet.

- Run your own VS Code server
- Code on your iPad or Surface


## Break: 10 min


## Advanced development Part II: tools that make you look like you know magic [45 minutes]

**Coding but faster** - We’ll do some exercises to show you how to speed up your coding practice.

- Keyboard shortcuts
- Bring your keymaps: vim/emacs/sublime/…
- Snippet extension

**Collaboration** - Here we’ll pair you up with someone else and go through some pair programming and code review exercises enabled by some powerful VS Code extensions. This exercise will require you to have a GitHub account.

- Pair programming with Live Share extension
- GitHub PR review extension

**Exercise**: Post a live share, build a new feature together, make commits to your project, open a pull request and review the code.

**Let AI code for you** - Of course, we cannot have a VS Code tutorial without showing this much talked about feature! We’ll go over some exercises to create new code using GitHub CoPilot’s VS Code extension.

- GitHub CoPilot: free for students and open-source contributors
- GitHub CoPilot Labs

**It’s Okay To Have Fun!** - Finally, we’ll show you some fun extensions that can help take the edge off of a busy workday.

- Vscode-pets
- Power Mode
- Music time

**Wrap-up & Epilogue** - It’s time to close out the tutorial and recap everything we’ve learned so far. We also want to end with some final remarks and recommendations.

- Recap of features/lessons
- Concluding remarks and recommendations
  - Where to look for more info and learning (docs, release notes, youtube channel)
  - Links on how to build your own VS Code extension
