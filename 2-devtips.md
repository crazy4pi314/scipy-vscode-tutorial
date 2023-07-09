# Scientific Python development tips and tricks

**Code navigation** - Learn how to speed up how you navigate through code.

- IntelliSense
- Symbol search (`@`, `@:`)
- [Balancing inward/outward](https://www.youtube.com/watch?v=NwqhFb4B5LU)
- Multi-line editing
- Find references
- Regex search
- Code transform
- Text selection
  - Select left/right: Ctrl+shift+arrow
  - Box select: alt

> **Exercise**: Explore code navigation
>
> 1. Create a new file `src/tutorial/hello.py` with a function `say_hello` that prints a message using the `emoji` library.
> 2. Output the text of Zen of Python into a file by running `python -c "import this" > src/tutorial/zen_of_python.md`.
> 3. Open the file and replace the word "is" with the word "was". How many keystrokes does it take to make this replacement in the editor?
> 4. Use regex search to find all sentences that have the pattern `\w+ better than \w+.`. Replace it with `is awesome!`.
> 5. Use Alt+ ↑ / ↓ to move the line "Readability counts." to the top.

**Running and testing code** - Now that we finally know our way around the editor it’s time to write and test some code! Here we’ll go through a few exercises that let you test the code you’ve written in the previous exercise and debug it.

- Shift + enter
- YAML extension + json/yaml schema = 💖
- Play button
- Unit tests extension
- Debugger

> **Exercise**: Debug code with tests
>
> 1. Create a new folder called `tests` and a new file `test_hello.py`.
> 2. Import the functions you've created in the first exercise using `from tutorial.hello import say_hello` and create a new function `test_say_hello` that calls `say_hello`.
> 3. Open the "Testing" menu by clicking on the vial icon in the primary side bar, click "Configure Python Tests" and choose "pytest". Pick the `tests` folder.
> 4. Run your test by clicking on the "Run Test" ▷ icon.
> 5. Add a new `name` input argument to the `say_hello` function. Run your test again. Can you fix the bug?

**Git and version control** - You’ve written some code - it’s time to push it upstream. We’ll go over some exercises that let you use the built-in Git tools to interact with the repository we cloned in the previous section.

- Git integration: branching, staging, committing, diff in-line
- Git Lens + integration with Git
- Pre-commit hooks
- GitHub actions (extensions to run them locally)

> **Exercise** Sign our yearbook!
>
> 1. Fork the [tutorial repo](https://aka.ms/scipy2023) to your GitHub account
> 2. Edit the file `yearbook2023.md` and add your favorite VS Code tip you've learned so far. Sign it with your GitHub handle.
> 3. Create a new branch using the menu `Branch` > `Create branch`, and name it `<your username>/yearbook-2023`.
> 4. Commit your changes to your new branch and push the changes using `Commit & Push`.
> 5. Create a PR to the origin repo, either with the GitHub PR extension or via the GitHub web interface so we can review and merge!

**Documentation** - Don't forget to document your work! Here we'll go over some tools in VS Code and GitHub to level up your docs.

- Sphinx + readthedocs
- LaTeX math rendering extension
- Docusaurus + github pages

**Data science tools** - After writing your code, let’s put it to use. Here we’ll cover some of VS Code’s specialized features for data science, and install some typical extensions that plug into the scientific Python ecosystem.

- Figures
- Jupyter notebooks: coding, testing and debugging
- Data wrangler
- Database queries
- [Data science profile](https://code.visualstudio.com/docs/editor/profiles#_data-science-profile-template)
