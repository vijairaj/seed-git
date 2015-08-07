# seed-git
Analysis of the first ever commit of the git source code gives a fairly good idea of the inner workings of the [git SCM](https://git-scm.com). The data structures and their representations have remained mostly unchanged and are still relevant. This repository exists to easily get started.

# Building with Makefile
Follow the standard build procedure:

    make

# Building with CMake
Follow the standard build procedure:

    mkdir build; cd build
    cmake ..
    make

# Debugging
One of the ways to analyze the source code is to step through the execution of the code line by line. [Qt Creator](https://wiki.qt.io/Category:Tools::QtCreator) make this easy because it can read CMake projects directly, so building and debugging is just one step away. Qt Creator can be installed from the distribution package or [downloaded directly](http://download.qt.io/official_releases/qtcreator/).

