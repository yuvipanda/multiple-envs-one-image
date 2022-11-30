# Multiple Conda Envs in One Image Example

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/yuvipanda/multiple-envs-one-image/HEAD)

This image provides an example of how multiple conda environments can be present in one docker image,
and users can easily switch between them.

There are three primary environments here:

1. The base notebook environment, in `environment.yml`. This contains the notebook package, any Jupyter frontends,
   as well as extensions to be used with JupyterLab - including [nb_conda_kernels](https://github.com/Anaconda-Platform/nb_conda_kernels).
2. A sample Python 3.11 environment, specified in `environment.python311.yml`.
3. A sample Python 3.7 environment, specified in `environment.python37.yml`.

The extra environments are initiated with a simple command in `postBuild`. Additional environments can be added
as necessary.
