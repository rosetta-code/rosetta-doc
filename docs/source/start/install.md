# Install Rosetta

Rosetta maintains different repositories for different programming languages. You can find instructions to install Rosetta for a language of your choice by selecting a language below.

:::{admonition} Some Adapters have language restrictions!
:class: attention
Some {term}`Adapters<Adapter>` can only be called using certain languages. For example, the Adapter for the Verasonics Vantage research ultrasound scanner system can only be called through Matlab because the Vantage API can only be called by Matlab. If you intend to work with a specific simulator or physical hardware configuration, make sure that you are choosing the version of Rosetta that's written in the appropriate language.
:::

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
