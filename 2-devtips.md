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
> 1. Create a new file `hello.py` in the `tutorial` package with a function `say_hello` that prints a message using the `emoji` library. Use IntelliSense to find the right function and order of input arguments from the library.
> 2. Output the text of Zen of Python into a file by running `python -c "import this" > zen_of_python.md`.
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
> 3. Open the "Testing" menu by clicking on the vial icon in the Activity bar, click "Configure Python Tests" and choose "pytest". Pick the `tests` folder.
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

- `autoDocstring` extension
- Sphinx
- LaTeX math rendering extension

> **Exercise** Document your code
>
> 1. Configure the `autoDocstring` extension to use `sphinx` as its Docstring format.
> 2. Add a docstring to the `say_hello` function you created in an earlier exercise.
> 3. (Optional) Run `sphinx-quickstart` to set up your Sphinx documentation and follow the steps in this [tutorial](https://github.com/melissawm/minimalsphinx) by @melissawm.
> 4. (Optional) Install the LaTeX Workshop extension (requires [TeX live](https://www.tug.org/texlive/)). Create a new folder `docs` with file `about.tex`. Start writing a page in [LaTeX](https://www.colorado.edu/aps/sites/default/files/attached-files/latex_primer.pdf) and explore the IntelliSense features.
>

**Data science tools** - After writing your code, let’s put it to use. Here we’ll cover some of VS Code’s specialized features for data science, and install some typical extensions that plug into the scientific Python ecosystem.

- Figures
- Jupyter notebooks: coding, testing and debugging
- Data wrangler
- Database queries
- [Data science profile](https://code.visualstudio.com/docs/editor/profiles#_data-science-profile-template)

> **Exercise** Data Science in VS Code
>
> 1. Create a new Data Science profile.
> 2. Open the `demo.ipynb` Jupyter Notebook.
> 3. Run the example cells in the notebook. Try adding a markdown cell and add some text, or add a code cell.
> 4. Open the example data file `bees.csv` using Data Wrangler and explore the dataset (source: [Bee-Gap: Ecology, Life-History, and Distribution of Bee Species in the United States 2017](https://www.sciencebase.gov/catalog/item/5bd868b2e4b0b3fc5ce9dadd)).
> Can you figure out which common plant name is most loved by all bee species recorded?
>
