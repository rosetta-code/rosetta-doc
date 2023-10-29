# Install Rosetta

## Get a copy of Rosetta
Rosetta maintains different repositories for different programming languages. You can find instructions to install Rosetta for a language of your choice by selecting a language below.

:::::{tab-set}
::::{tab-item} Matlab
  :sync: tabMatlab

  **Requires:** Matlab R2019a or later.

  Go to [the Git repository](https://github.com/rosetta-code/rosetta-matlab) to download a stable release of Rosetta for Matlab.

  Rosetta for Matlab is still under development. Once it is operational, we intend to also distribute it on the [Matlab File Exchange](https://www.mathworks.com/matlabcentral/fileexchange). In the meantime, please follow our development on the Git repository for Rosetta, and contribute if you're interested.

  **Note:** Core portions of the current implementation of Rosetta for Matlab are written only using basic functions (i.e. without relying on any toolboxes or add-ons). Given this, Rosetta is expected to be functional using GNU Octave. However, this has not been tested yet; please do so at your own risk and freel free to submit pull requests if you encounter any problems.
::::
::::{tab-item} Python
  :sync: tabPython

  **Requires:** Python 3.10 or later. See Conda Environments or Pip Requirements file for dependencies.

  Go to [the Git repository](https://github.com/rosetta-code/rosetta-py3) to download a stable release of Rosetta for Python.

  Rosetta for Python is still under development. Once it is functional at a minimally useful level, we intend to also distribute it on PyPi (for Pip) and conda-forge (for Anaconda). In the meantime, please follow our development on the Python 3 repository for Rosetta, and contribute if you're interested.
::::
:::::

:::{admonition} Some Adapters have language restrictions!
  :class: attention
  Some {term}`Adapters<Adapter>` can only be called using certain languages. For example, the Adapter for the Verasonics Vantage research ultrasound scanner system can only be called through Matlab because the Vantage API can only be called by Matlab. If you intend to work with a specific simulator or physical hardware configuration, make sure that you are choosing the version of Rosetta that's written in the appropriate language.
:::

### Get Rosetta for development
<!--Note: this heading name must be retained due to a link in contribute/index.html-->
You can create an isolated copy of Rosetta for the language of your choice by creating your own {term}`repositories<Repository>` using {term}`Git`. This will let you pull (get the latest updates) from our repo and push (share potential changes you make) in a controlled and convenient way. To set this up:

1. [Fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) the latest development branch of your preferred language's Rosetta repo. To do this, you can create your own GitHub account, go to the repository, select the `dev` branch, and click "fork".

2. If you do not already have them, install Git by following instructions on [its website](https://git-scm.com/) as well as an {term}`IDE` of your choice. Rosetta strongly recommends [Microsoft Visual Studio Code (VSCode)](https://code.visualstudio.com/) as an IDE due to its flexibility and ease of use.

3. Open a command line window (Windows) or console (Mac/Linux) and navigate to the folder where you want a folder for Rosetta to be created. This is usually done using the `cd` command.

4. {term}`Clone` the Rosetta repo of your choice using the instructions below this list.

5. Configure your IDE to incorporate the following text formatters:
  * **Black** - an opinionated tool that makes Python code compliant with the PEP8 standard
  * **Prettier** - a multi-purpose code formatter to standardize how code in all other languages are written
<!--for Matlab, consider MBeautifier or MISS_HIT-->

:::{admonition} Configuring VSCode for Rosetta
:class: info

Rosetta repositories contain VSCode [workspace files](https://code.visualstudio.com/docs/editor/workspaces) that allow extensions to be downloaded and installed in a self-contained way. You can simply use the VSCode folder (`.vscode`) in the root folder to install the recommended extensions.
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

  We can use Python's virtual environment (`venv`) feature. This involves defining a virtual environment in a folder called `env` inside our repository. To do so, navigate your console into the newly-created folder, then run:
  
  :::{code-block} python
  python3 -m venv env
  :::

  We can install all Rosetta-relevant Python packages in our virtual environment using the `requirements.txt` file:

  :::{code-block} python
  pip install -r requirements.txt
  :::

  ???

  :::{code-block} python
  pip install -e .
  :::
  :::::

  :::::{dropdown} Develop Rosetta using Anaconda

  We can create virtual environments using Conda, which comes in two variants:
  
  * **[Anaconda](https://www.anaconda.com/download)**, which pre-downloads many popular packages but can take up an excessive amount of storage space due to the sheer size of its content, or;
  
  * **[Miniconda](https://docs.conda.io/projects/miniconda/en/latest/index.html#quick-command-line-install)**, the lightweight version of Anaconda that does not come with a GUI or pre-downloaded packages.
  
  Once you download the Conda platform of your choice, we can use the `environment.yml` file in the Rosetta repo to create a Conda environment called `env-name` that is populated with all necessary packages. To do so, run:

  :::{code-block} python
  conda env create -n env-name -f environment.yml
  :::
  
  If you want to develop Rosetta for Python using a Conda-based package manager, your ***base*** environment needs to have `conda-build`, the tools to develop new packages using Conda.

  To create a Conda environment 

  :::{code-block} python
  conda-install -n base conda-build
  conda-develop /path/to/git/repo/
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


## Verify that Rosetta works
To use Rosetta, we must make sure that your copy of it is installed *and* recognized. We will make sure that Rosetta can be added to relevant {term}`namespaces<Namespace>` for your platform, then ensure that it can run.

:::::::{tab-set}
::::::{tab-item} Matlab
  :sync: tabMatlab
  
  To call Rosetta, we must either:
  
  1. [Manually add our copy of Rosetta to Matlab's search paths](https://www.mathworks.com/help/matlab/ref/addpath.html) through the `addpath` function, or;
  
  2. [Automatically have Matlab recognize Rosetta on startup](https://www.mathworks.com/help/matlab/matlab_env/add-folders-to-matlab-search-path-at-startup.html) by changing its search paths.

  If you manually installed Matlab at a location you chose, simply use the path to that folder as input arguments for either of the two approaches above.

  If Rosetta was installed using the Matlab File Exchange, its default location depends on the operating system that is running Matlab. The default paths are as follows:

  :::::{tab-set}
  ::::{tab-item} Windows
  :sync: tabOsWin
  Note that the default path for Matlab's add-ons depend on your username. Replace the string `username` in the path below with your username:

  :::{code-block} none
  C:\Users\username\AppData\Roaming\MathWorks\MATLAB Add-Ons` 
  :::
  ::::

  ::::{tab-item} macOS
  :sync: tabOsMac

  :::{code-block} none
  ~/Library/Application Support/MathWorks/MATLAB Add-Ons` 
  :::
  ::::

  ::::{tab-item} Linux
  :sync: tabOsLinux

  :::{code-block} none
  ~/MATLAB Add-Ons
  :::
  ::::
  :::::
::::::

::::::{tab-item} Python
  :sync: tabPython

  Rosetta may be used in Python simply by importing it into the relevant {term}`namespace<Namespace>`. This means that a Python file or Jupyter notebook can use Rosetta if it starts with the following statements:

  :::{code-block} python
  import rosetta_py as ros
  :::

::::::
:::::::

