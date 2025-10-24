# Python/Conda
Python is a general-purpose programming language widely used in data science, artificial intelligence, and increasingly in mathematical research. Its rich ecosystem of libraries—such as **NumPy** (linear algebra and matrix operations), **SciPy** (scientific computing), **SymPy** (symbolic mathematics), **TensorFlow** (machine learning), **Pandas** (data analysis), and **matplotlib** (visualization)—makes it an ideal language for research applications.

For the Sessie Research Group, we’ve developed a generalized causal engine in a custom Python framework called RuleFlow. RuleFlow implements subsets of causal behavior tailored for robust analysis of Sessies. To use RuleFlow, you’ll need to set up a dedicated Python environment using **Conda**.

**Conda** is a lightweight command-line tool that simplifies managing multiple Python versions, packages, and dependencies across projects. It’s especially useful in research settings where each project may require a unique configuration. With Conda, we can maintain isolated, reproducible environments for each research module.

While any text editor can be used to write Python code, we recommend using an **IDE** (Integrated Development Environment) for its advanced features—such as smart code completion, debugging tools, visualization support, and seamless integration with **Jupyter Notebooks**. Jupyter Notebooks allow you to combine runnable Python code with markdown explanations in a single document, making them ideal for research workflows. They function similarly to Mathematica Notebooks, offering an interactive and readable format for both computation and documentation.

## Setting up Conda and Python
### 1. Install Conda

We recommend installing **Miniconda** (a lightweight version of Anaconda) unless you specifically need the full Anaconda distribution.

- Download Miniconda from the [official site](https://docs.conda.io/en/latest/miniconda.html).
- Follow the installer instructions for your operating system (Windows, macOS, Linux).
- After installation, verify Conda is available:

```bash
conda --version
```

### 2. Create a New Environment

Each project should have its own environment. For example, to create an environment named `sessie-env` with Python 3.14:

```bash
conda create -n sessie-env python=3.14
```

Activate the environment:

```bash
conda activate sessie-env
```

Deactivate when finished:

```bash
conda deactivate
```

### 3. Install Packages
In Python, software add‑ons are called packages—collections of code that provide extra functionality, such as numerical computing (numpy), data analysis (pandas), or visualization (matplotlib). While Conda can install many packages, Python also comes with its own package manager called pip. Pip allows you to download and install packages from the [Python Package Index (PyPI)](https://pypi.org/), which hosts thousands of open‑source libraries. For example, running `pip install numpy` will add the popular math library to your environment. Beginners should remember that packages installed with pip are tied to the active environment, so it’s best to always activate the correct Conda environment before using pip. Custom packages we develop (like RuleFlow) will instead be "installed" using Git commands (documentation for installing such packages should be written on the repository).

Once inside your environment, install required libraries. For example:

```bash
conda install numpy pandas matplotlib
```

If a package isn’t available via Conda, you can still use `pip`:

```bash
pip install sympy
```

### 4. Export and Reproduce Environments

To share your environment with others (or reproduce it later), export it to a YAML file:

```bash
conda env export > environment.yml
```

Others can recreate the same environment with:

```bash
conda env create -f environment.yml
```

### 5. Verify Python Setup

Check that Python is installed correctly in your environment:

```bash
python --version
```

You can now run Python scripts or launch an interactive shell:

```bash
python
```

### Best Practices

- Always activate the correct environment before running code.
- Keep environments project‑specific to avoid conflicts.
- Use `environment.yml` files for reproducibility across the research group.
- Combine Conda with Jupyter Notebooks for interactive workflows.


## Setting up an IDE
An **IDE (Integrated Development Environment)** streamlines coding by providing features like syntax highlighting, debugging, version control integration, and direct environment management. For Python development, we recommend **PyCharm** and **Visual Studio Code (VS Code)**.

### PyCharm
[PyCharm](https://www.jetbrains.com/pycharm/) (by JetBrains) offers a **Professional Edition** that is free for students through the [JetBrains Student Program](https://www.jetbrains.com/community/education/#students). They also offer a **completely free and open-source version**. PyCharm provides advanced features such as Jupyter Notebook integration, scientific mode, seamless GitHub integration, and much more. PyCharm is easier to setup and use than VS Code due not having to install multiple extensions and configure settings; everything works out-of-the-box.

- To use a Conda environment in PyCharm:
    1. Go to _Settings → Project → Python Interpreter_.
    2. Click the gear icon → _Add Interpreter_.
    3. Select _Conda Environment_ and choose the environment you created.

### Visual Studio Code
[VS Code](https://code.visualstudio.com/) is a lightweight, extensible editor with strong Python support through the [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python). It integrates well with GitHub and has a large ecosystem of plugins.

- To use a Conda environment in VS Code:
    1. Install the Python extension.
    2. Open the Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`).
    3. Search for _Python: Select Interpreter_ and choose your Conda environment.

Both IDEs allow you to run code directly within the selected Conda environment, ensuring consistency with your project dependencies.


## Setting up Jupyter Notebooks
Jupyter Notebooks are interactive documents that combine runnable Python code, explanatory text (written in Markdown), and visualizations in a single file. They function much like Mathematica notebooks, allowing you to mix computation with narrative and results in a readable, reproducible format. Both VS Code (with the Jupyter extension) and PyCharm Professional support running Jupyter Notebooks directly, making it easy to test code, document workflows, and share results. Best practices include keeping notebooks focused on a single task or experiment, using Markdown cells for clear explanations, and exporting results to version‑controlled scripts when workflows become stable. This approach ensures that notebooks remain both a research tool and a communication medium.

**Learn More:**
- [Jupyter Notebook support in PyCharm (JetBrains Docs)](https://www.jetbrains.com/help/pycharm/jupyter-notebook-support.html)
- [Jupyter Notebooks in VS Code (Microsoft Docs)](https://code.visualstudio.com/docs/datascience/jupyter-notebooks)
- [Project Jupyter Documentation](https://docs.jupyter.org/)
- [Installing Jupyter](https://jupyter.org/install)
- [Try Jupyter in your browser](https://docs.jupyter.org/en/latest/start/index.html)


## Tips for Getting Started
Python is designed to be user‑friendly, so the best way to learn is by writing small pieces of code and experimenting. Start by opening a Python shell or creating a simple script in your IDE. Focus on the basics: variables, loops, functions, and working with built‑in data types like lists and dictionaries. Most uses of our custom RuleFlow tool will require very little knowledge of Python. In addition, lots of examples will be provided for using in-house python tools that we develop.

Here’s a simple example to try in your environment:
```python
# A basic Python example
def greet(name):
    return f"Hello, {name}!"

for person in ["Alice", "Bob", "Charlie"]:
    print(greet(person))
```

**Learn More:**
- [Python For Beginners (Python.org)](https://www.python.org/about/gettingstarted/)  
- [The Python Tutorial (Official Docs)](https://docs.python.org/3/tutorial/index.html)  
- [W3Schools Python Tutorial](https://www.w3schools.com/python/)  
- [LearnPython.org Interactive Tutorial](https://www.learnpython.org/)  
- [Real Python Tutorials](https://realpython.com/)  
