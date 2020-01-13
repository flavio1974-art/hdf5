

Installation
------------

Make sure that you have the following Python packages installed:

-   python 3
-   jupyter
-   NumPy
-   h5py
-   PyTables
-   pandas
-   matplotlib
-   cartopy

For (ana)conda users an enviroment (called hdf5) with all required packages can be created using the provided environment.yml. On windows:

    > conda env create -f environment-windows.yml

Activate the environment with:

    > activate hdf5

Or Linux/Mac:

    $ conda env create -f environment.yml
    $ source activate hdf5

Now run the test script:

    > python test_env.py

Verify the jupyter notebook server works:

    > jupyter notebook

And run the 'test\_env.ipynb' notebook.

Python 3
--------

The notebooks are written and testing on python 3 only. Using python 2.7 is possible but not recommended.

Optional HDF5 1.10 enviroment (Linux/Mac only)
----------------------------------------------

For notebook 10 (Parallel HDF5) h5py built against HDF5 v1.10 is needed with and without Parallel HDF5 enabled. More on this in the tutorial.

If possible create a (python 2.7!) enviroment with HDF5 1.10 and h5py:

    $ conda create -n hdf5_1-10 python=2.7
    $ source activate hdf5_1-10
    $ conda install -c cfel hdf5 h5py

And for Parallel HDF5 and h5py:

    $ conda create -n hdf5-mpi python=2.7
    $ source activate hdf5_1-10
    $ conda install -c cfel hdf5-mpi h5py-mpi mpi4py

NO se enoje nadie por ser pirata
