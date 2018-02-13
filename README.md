# gsa2017

This repository was born as a stripped-down fork of the King's Geocomputation [repository](https://github.com/kingsgeocomp/geocomputation). Its purpose it to keep track of changes to the `.yml` file used for setting up a [conda](https://conda.io/docs/) environment which turnecd out to be necessary during Spatial Analysis tutorials in Spring 2018. It should provide a place where an up-to-date working version of the environment can be retrieved and installed from, via:

```
conda env create -f <fname>
```

This will create a new environment called `gsa2017sa` intended to be used for Spatial Analysis tutorials. This will probably need to be augmented to also accomodate all modules needed for Applied Geocomputation and Spatial Analysis. E.g. At the time of writing, SOMPY is not included in the `gsa2017sa` environment. 

## Change log
- Attempted a compromise between the forked geocomputation version of `setup.yml`and the version Chen posted to KEATS on 2017-02-01 which includes a working version of `georasters` and is tested on Windows. There may be some parts of this merge which don't work for modules needed for Applied Geocomputation, including SOMPY.


