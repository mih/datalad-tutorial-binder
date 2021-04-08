# Run DataLad tutorials on Binder

## Run the tutorial notebook

To open a Jupyter Notebook with the DataLad tutorial in your browser, click the following link:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/datalad-handbook/datalad-tutorial-binder/HEAD?filepath=code%2FOHBM.ipynb)

By doing so, everything will be set up for you in the cloud (via [MyBinder](https://mybinder.org/)), so you don't have to worry about installation of DataLad or other package dependencies.

You can start working through the tutorial right away! :smile:

## What is this?

This repository contains the Binder setup required for running Jupyter Notebooks that use DataLad.
The repository was imported from [here](https://github.com/marianne-aspbury/openmr2021-dataviz-workshop-python),
and further updates were then implemented:

1. Convert the [`OHBM.rst`](https://github.com/datalad-handbook/book/blob/master/docs/code_from_chapters/OHBM.rst) tutorial file into a Jupyter Notebook, using [sphinxcontrib-jupyter](https://github.com/QuantEcon/sphinxcontrib-jupyter).
2. Add the converted notebook to the current repository, under `code/`
3. Update the notebook to streamline the execution of terminal/bash commands (add line and cell magics)

*Note: the majority of the notebook code executes as expected, apart from places where `git clone` is used with `ssh`*

## TODO

- Figure out problem with using `git clone` via `ssh` on Binder
- Update either `rst` file or conversion process so that the edits mentioned in point 3 above would not be necessary
- Automate building Jupyter notebook directly from [book content](https://github.com/datalad-handbook/book)