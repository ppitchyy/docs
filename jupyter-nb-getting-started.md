# Jupyter Notebook

# [Installing Jupyter Notebook](http://jupyter.readthedocs.io/en/latest/install.html)

Installing with [Anaconda](https://www.anaconda.com/download/):
* To change Python version (e.g. to Python 3.5), run this command in the root environment: `conda install python=3.5`
* Run Jupyter Notebook: `jupyter notebook`

Installing with Pip:
* For Python3: `pip3 install --upgrade pip` then `pip3 install jupyter`
* For Python2: `pip install jupyter`


### Kernels:
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
