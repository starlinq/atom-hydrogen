# Python based development with Atom-Hydrogen
Tutorial on using Atom editor with hydrogen package for Python based development as jupyter notebook

This is a great alternative for interactive programming to common Visual Studio Code with well-known Python and Jupyter extensions.

There are some advantages of this approach:

- Full support of Jupyter API without any hassle (file with regular .py extension, markdown and code cells are separated with simple '# %%' marks, at the same time it shows a generated output for true interactive programming)
- Supports both python and conda environments
- Requires less resources (so accordingly consumes less computer memory)

## Using Anaconda/Miniconda environments

Under Windows OS, after installation of Anaconda3 (with Python version 3.X support), ones open Anaconda3 Prompt window, then we can specify any command.

In first we have to create a new environment

```
conda create --name mypyenv python=3.8
conda install -n mypyenv jupyter
```
In the first command line we specified a Python version otherwise the latest OS-supported version will be installed.

Before using we have to activate the created environment:

```
conda activate mypyenv
```
The next step is very important in adding support of Jupyter kernel to the environment
```
python -m ipykernel install --user --name mypyenv
```
If everything is okay, the following message will be generated varying on your platform, e.g. for Windows OS

```
Installed kernelspec mypyenv in C:\Users\yourusername\AppData\Roaming\jupyter\kernels\mypyenv
```
