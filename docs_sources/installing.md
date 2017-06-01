TPOT is built on top of several existing Python libraries, including:

* [NumPy](http://www.numpy.org/)

* [SciPy](https://www.scipy.org/)

* [scikit-learn](http://www.scikit-learn.org/)

* [DEAP](https://github.com/DEAP/deap)

* [update_checker](https://github.com/bboe/update_checker)

* [tqdm](https://github.com/tqdm/tqdm)


Most of the necessary Python packages can be installed via the [Anaconda Python distribution](https://www.continuum.io/downloads), which we strongly recommend that you use. We also strongly recommend that you use of Python 3 over Python 2 if you're given the choice.

NumPy, SciPy, and scikit-learn can be installed in Anaconda via the command:

```Shell
conda install numpy scipy scikit-learn
```

DEAP, update_checker, and tqdm can be installed with `pip` via the command:

```Shell
pip install deap update_checker tqdm
```

**For the Windows users**, the pywin32 module is required if Python is NOT installed via the [Anaconda Python distribution](https://www.continuum.io/downloads) and can be installed with `pip`:

```Shell
pip install pywin32
```

**Optionally**, you can install [XGBoost](https://github.com/dmlc/xgboost) if you would like TPOT to use the eXtreme Gradient Boosting models. XGBoost is entirely optional, and TPOT will still function normally without XGBoost if you do not have it installed.

```Shell
pip install xgboost
```

If you have issues installing XGBoost, check the [XGBoost installation documentation](http://xgboost.readthedocs.io/en/latest/build.html).

**Note: For now, TPOT only supports xgboost 0.6a2. Please find the source codes [under v0.60 tag of xgboost's GitHub](https://github.com/dmlc/xgboost/tree/v0.60) if you need build xgboost**

If you plan to use the [TPOT-MDR configuration](https://arxiv.org/abs/1702.01780), make sure to install [scikit-mdr](https://github.com/EpistasisLab/scikit-mdr) and [scikit-rebate](https://github.com/EpistasisLab/scikit-rebate):

```Shell
pip install scikit-mdr skrebate
```

Finally to install TPOT itself, run the following command:

```Shell
pip install tpot
```

Please [file a new issue](https://github.com/rhiever/tpot/issues/new) if you run into installation problems.