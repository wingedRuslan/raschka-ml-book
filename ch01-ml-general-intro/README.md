Python Machine Learning - Code Examples


##  Chapter 1: Giving Computers the Ability to Learn from Data


---



## For Existing Conda Users: Creating a New Conda Environment (Optional)



If you are already a conda user, you can skip the next section and get all the recommended package versions in a fresh conda environment (called "pyml-book") via


```
make -f Makefile
```

from the main folder in this repository.



## Setting Up Your Python Environment (Manually)

**Conda**

If you are using conda (we recommend installing conda via [Miniforge](https://github.com/conda-forge/miniforge)), you can create a new environment as follows:

```bash
conda create -n "pyml-book" python=3.9 numpy=1.21.2 scipy=1.7.0 scikit-learn=1.0 matplotlib=3.4.3 pandas=1.3.2
```

After creating this environment, you can activate it via

```bash
conda activate "pyml-book"
```



**Pip and virtualenv**

If you prefer using `pip`, you can go ahead and install the required packages via

```bash
pip install numpy==1.21.2 scipy==1.7.0 scikit-learn==1.0 matplotlib==3.4.3 pandas==1.3.2
```

However, we additionally recommend creating a new virtual environment. 
You can create a new virtual environment with a specific Python version using [virtualenv](https://virtualenv.pypa.io/en/latest/) as follows:

```bash
pip install virtualenv
cd /path/to/where/you/want/your/environment
virtualenv pyml-book
source pyml-book/bin/activate 
```

After activating your environment, you can install the required packages via

```bash
pip install numpy==1.21.2 scipy==1.7.0 scikit-learn==1.0 matplotlib==3.4.3 pandas==1.3.2
```







## Checking Your Python Environment

To verify that your Python environment is set up, run the [`../python_environment_check.py`](../python_environment_check.py) script provided in the main folder of this repository.

You can run the `python_environment_check.py` script via

    python python_environment_check.py

Shown below is an example output:

```python
(base) sebastian@MacBook-Air ~/Desktop/Python-Machine-Learning-PyTorch-Edition/ch01 % python ../python_environment_check.py
[OK] Your Python version is 3.9.6 | packaged by conda-forge | (default, Jul 11 2021, 03:35:11)
[Clang 11.1.0 ]
[OK] numpy 1.21.2
[OK] scipy 1.7.0
[OK] matplotlib 3.4.3
[OK] sklearn 1.0
[OK] pandas 1.3.2
```


## Jupyter Notebooks


Compared to regular .py scripts, Jupyter notebooks allow us to have everything in one place:

- Our code.
- The results from executing the code.
- Plots of our data.
- Documentation supporting the handy Markdown and LaTeX syntax for typing and rendering mathematical notation.

Please see the https://jupyter.org/install website for the latest installation instructions.

Jupyter Lab can be installed via 

```bash
conda install -c conda-forge jupyterlab
```

or 

```bash
pip install jupyterlab
```

All code examples found in this book are also available via .py script files (which were converted from the Jupyter notebooks to ensure that they contain the identical code.)
