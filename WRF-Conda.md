Anaconda 3 installs a lot of useful packages by default in the main environment

1. Download the last anaconda package for the last python 3 :

`wget https://repo.continuum.io/archive/Anaconda3-4.4.0-Linux-x86_64.sh`

2. Install the python 3 version of Anaconda (Python 2.7 is still accessible from Anaconda 3):

`bash Anaconda3-4.3.1-Linux-x86_64.sh`

Answer Yes to every questions, it will create a base repository named anaconda3

3. Refresh the bashrc so conda command are recognized

`source ~/.bashrc` 

4. Create a new virtualenvironment

`conda create --name WRF numpy scipy xarray`

Since we built Anaconda 3, the default python's version is 3, to get a python 2.7 we can just add:
`python==2.7` to the conda create command

5. Activate the newly created environment

`source activate WRF` (then ipython is accessible)

The virtual environment is now active, to install a new package : `conda install package` 

Or if it is not yet inside the anaconda system (if previous command failed):`pip install package`

To get out of the environment : source deactivate
