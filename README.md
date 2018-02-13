# gsa2017

This repository was born as a stripped-down fork of the King's Geocomputation [repository](https://github.com/kingsgeocomp/geocomputation). Its purpose it to keep track of changes to the `.yml` file used for setting up a [conda](https://conda.io/docs/) environment which turnecd out to be necessary during Spatial Analysis tutorials in Spring 2018. It should provide a place where an up-to-date working version of the environment can be retrieved and installed from, via:

```
conda env create -f https://raw.githubusercontent.com/alanecode/gsa2017/master/setup.yml
```

This will create a new environment called `gsa2017sa` intended to be used for Spatial Analysis tutorials. This will probably need to be augmented to also accomodate all modules needed for Applied Geocomputation and Spatial Analysis. E.g. At the time of writing, SOMPY is not included in the `gsa2017sa` environment. 

Remember: when installing on one of KCL's Windows machines, it is necessary to run the following commands in the Anaconda prompt to persuade Jupyter to provide the new environment as a kernel option:

```
activate gsa2017sa
python -m ipykernel install --name gsa2017sa --display-name "gsa2017sa"
```

## Change log
- Attempted a compromise between the forked geocomputation version of `setup.yml`and the version Chen posted to KEATS on 2017-02-01 which includes a working version of `georasters` and is tested on Windows. There may be some parts of this merge which don't work for modules needed for Applied Geocomputation, including SOMPY.

- Added the module [`pointpats`](https://github.com/pysal/pointpats) installed using `pip`. This module contains the `PointPattern` object which was formerly included in the PySAL module `pysal.contrib.points.pointpattern` before the PySAL [refactoring](https://github.com/pysal/pysal/wiki/PEP-13:-Refactor-PySAL-Using-Submodules) effort. After this inclusion, it should be possible to import `PointPattern` using `from pointpats import PointPattern`.

## TODO
- 2017-02-13 Test `gsa2017sa` on Windows


