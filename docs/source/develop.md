# Get Rosetta for development

<!--Note: this heading name must be retained due to a link in contribute/index.html-->

You can create an isolated copy of Rosetta for the language of your choice by creating your own {term}`repositories<Repository>` using {term}`Git`. This will let you pull (get the latest updates) from our repo and push (share potential changes you make) in a controlled and convenient way. To set this up:

1. [Fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) the latest development branch of your preferred language's Rosetta repo. To do this, you can create your own GitHub account, go to the repository, select the `dev` branch, and click "fork".

2. If you do not already have them, install Git by following instructions on [its website](https://git-scm.com/) as well as an {term}`IDE` of your choice. Rosetta strongly recommends [Microsoft Visual Studio Code (VSCode)](https://code.visualstudio.com/) as an IDE due to its flexibility and ease of use.

3. Open a command line window (Windows) or console (Mac/Linux) and navigate to the folder where you want a folder for Rosetta to be created. This is usually done using the `cd` command.

4. {term}`Clone` the Rosetta repo of your choice using the instructions below this list.

5. Configure your IDE to incorporate the following text formatters:

- **Black** - an opinionated tool that makes Python code compliant with the PEP8 standard
- **Prettier** - a multi-purpose code formatter to standardize how code in all other languages are written
<!--for Matlab, consider MBeautifier or MISS_HIT-->

:::{admonition} Configuring VSCode for Rosetta
:class: info

Rosetta repositories contain VSCode settings and extensions files that allow extensions to be downloaded and installed in a self-contained way. You can simply use the VSCode folder (`.vscode`) in the root folder to install the recommended extensions.
:::

The appropriate way to clone Rosetta depends on your desired language:

:::::::{tab-set}
::::::{tab-item} Matlab
:sync: tabMatlab

The concept of discrete development environments does not exist for Matlab. This means we can just directly run:

:::{code-block} none
git clone https://github.com/rosetta-code/rosetta-matlab.git
:::
::::::
::::::{tab-item} Python
:sync: tabPython

For Python, we can start by creating a local repo by running:

:::{code-block} none
git clone https://github.com/rosetta-code/rosetta-py3.git
:::

Python best practices suggest that we should create an isolated environment for each project. We can do so by creating a virtual environment in one of two ways: using a **Pip `venv`** or **Anaconda**.

:::::{dropdown} Develop Rosetta using Pip Virtual Environment

We can use Python's virtual environment (`venv`) feature. This involves defining a virtual environment in a folder called `env-name` inside our repository. To do so, navigate your console into the newly-created folder, then run:

:::{code-block} python
python3 -m venv env-name
:::

We can install all Rosetta-relevant Python packages in our virtual environment using the `requirements.txt` file:

:::{code-block} python
pip install -r requirements.txt
:::

If we want to treat the repo that we cloned as its own package as if we downloaded it from Pip, we can run:

:::{code-block} python
pip install -e .
:::
:::::

:::::{dropdown} Develop Rosetta using Anaconda

We can create virtual environments using Conda, which comes in two variants:

- **[Anaconda](https://www.anaconda.com/download)**, which pre-downloads many popular packages but can take up an excessive amount of storage space due to the sheer size of its content, or;

- **[Miniconda](https://docs.conda.io/projects/miniconda/en/latest/index.html#quick-command-line-install)**, the lightweight version of Anaconda that does not come with a GUI or pre-downloaded packages.

Once you download the Conda platform of your choice, we can use the `environment.yml` file in the Rosetta repo to create a Conda environment called `env-name` that is populated with all necessary packages. To do so, run:

:::{code-block} python
conda env create -n env-name -f environment.yml
:::

Your **_base_** environment also needs to have `conda-build`, the tools to develop new packages using Conda. With this, we can call `conda-develop` to install the Rosetta package for Python in "development mode" from the repo that we just cloned.

:::{code-block} python
conda-install -n base conda-build
conda-develop ./rosetta-py3
:::
:::::

::::::
::::::{tab-item} JavaScript
:sync: tabJs

Rosetta for JavaScript is envisioned as a nice-to-have goal for the future. We intend to make sure that Rosetta works in a useful way using Matlab and Python, first, before expanding to other coding environments.
::::::
::::::{tab-item} Julia
:sync: tabJulia

Rosetta for Julia is envisioned as a nice-to-have goal for the future. We intend to make sure that Rosetta works in a useful way using Matlab and Python, first, before expanding to other coding environments.
::::::
::::::{tab-item} C++
:sync: tabC

Rosetta for C++ is envisioned as a nice-to-have goal for the future. We intend to make sure that Rosetta works in a useful way using Matlab and Python, first, before expanding to other coding environments.
::::::
:::::::
