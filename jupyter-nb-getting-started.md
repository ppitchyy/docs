# Jupyter Notebook

# [Installing Jupyter Notebook](http://jupyter.readthedocs.io/en/latest/install.html)

Installing with [Anaconda](https://www.anaconda.com/download/):
* To change Python version (e.g. to Python 3.5), run this command in the root environment: `conda install python=3.5`
* Run Jupyter Notebook: `jupyter notebook`

Installing with Pip:
* For Python3: `pip3 install --upgrade pip` then `pip3 install jupyter`
* For Python2: `pip install jupyter`


### Kernels: 
* [IPython](https://en.wikipedia.org/wiki/IPython) (Interactive Python) is used as a kernel for Jupyter
* If you are running Jupyter on Python 2 and want to set up a Python 3 kernel: 
```
python3 -m pip install ipykernel
python3 -m ipykernel install --user
```

* or manually register ipython kernels (Change to version 2.7 to do the other way round (running Jupyter on Python 3 and want to set up Python 2 kernel))
```
conda create -n py36 python=3.6
source activate py36
conda install notebook ipykernel
ipython kernel install --user
```

# [Starting the Notebook Server](https://jupyter.readthedocs.io/en/latest/running.html#running)

* Open specific Notebook: `jupyter notebook mynotebook.ipynb`
* Start the Notebook using a custom IP or port (default is 8888): `jupyter notebook --port 9999`
* Start the Notebook without opening a web browser: `jupyter notebook --no-browser`
* Get help: `jupyter notebook --help`

