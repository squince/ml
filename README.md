## Run
1. In each terminal window/tab you want to run with this environment,
   you must source the environment first.
   * `source activate myml`
1. Then run jupyter
   * `jupyter notebook`
 
# Installation and Environment Setup
1. Anaconda is recommended as the environment and package manager.
   * https://www.continuum.io/download://www.continuum.io/downloads
1. Once installed, create and activate an environment within which you'll install dependencies
   * `conda create --name myml` - creates a new python environment
   * `source activate myml` - activates that environment
   * `conda env list` - displays all python environments and denotes which is active
1. You'll need to be sure you have Python 3.5.x and all dependencies installed (some dependencies are not 3.6.x compatible)
   * Install the dependencies listed in `./requirements.txt` using the following Anaconda command `conda install --file requirements.txt`
   * **Or**, you can install each (or new ones) individually using command line format `conda install python=3.5.3` 
   * And, you can search for dependency names using `conda search <some word>`
1. Then you have to explicitly tell Jupyter about this environment by creating a new kernel
   * `python -m ipykernel install --user --name myml --display-name "Python (myml)"` 
