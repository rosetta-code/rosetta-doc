# Verify that Rosetta works

To use Rosetta, we must make sure that your copy of it is installed _and_ recognized. We will make sure that Rosetta can be added to relevant {term}`namespaces<Namespace>` for your platform, then ensure that it can run.

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
