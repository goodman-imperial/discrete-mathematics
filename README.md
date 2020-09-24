# discrete-mathematics
Imperial College EEE discrete mathematics course

The easiest way to use these notebooks if you have a Google account is to launch it in Google Colab, using the button below:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/goodman-imperial/discrete-mathematics)

Once you've launched it, you can make a copy into your Google Drive that you can save.

Alternatively, if you don't have a Google account you can run it in Binder, although there is no option to save a copy. Use the button below.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/goodman-imperial/discrete-mathematics/master)

Or, if you're comfortable with Python, you can install and run Python locally. My recommended technique is as follows:

Firstly, install [Miniconda](https://docs.conda.io/en/latest/miniconda.html) for Python 3.

If you're using Windows, you'll need to
[install the Microsoft Build Tools](https://wiki.python.org/moin/WindowsCompilers#Compilers_Installation_and_configuration)
and [Git for Windows](https://git-scm.com/download/win). On Linux you probably don't need to do anything,
and I have no idea about Macs but they're a bit like Linux so hopefully it's simple.

Next, set up Conda to use ``conda-forge`` for binary distributions, by running this at the terminal.

```
conda config --add channels conda-forge 
conda config --set channel_priority strict
```

Create a Jupyter notebook virtual environment:

```
conda create --name jupyter python=3 jupyter jupyter_contrib_nbextensions nb_conda_kernels jupytext matplotlib
```

Checkout the repository:

```
git clone https://github.com/goodman-imperial/discrete-mathematics.git discrete-mathematics
```

From the cloned directory, create a virtual environment called ``dmclass`` for this project:

```
conda create -f environment.yml
```

Now activate the Jupyter environment and run the Jupyter server:

```
conda activate jupyter
jupyter notebook
```
