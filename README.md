# Python based development with atom-hydrogen workflow
Tutorial on using Atom editor with hydrogen package for Python based development as jupyter notebook

This is a great alternative for interactive programming to common Visual Studio Code with well-known Python and Jupyter extensions.

There are some advantages of this approach:

- Full support of Jupyter API without any hassle (file with regular .py extension, markdown and code cells are separated with simple '# %%' marks, at the same time it shows a generated output for true interactive programming)
- Supports both python and conda environments
- Requires less resources (so probably consumes less computer memory)

## Using Anaconda/Miniconda environments

In first we have to create a new environment

```
conda create --name mypyenv python=3.8
```
In last command we specified a Python version otherwise the latest OS-supported version will be installed.

Before using we have to activate the created environment:

```
conda activate mypyenv
```

