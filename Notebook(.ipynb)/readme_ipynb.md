## **NOTE**
***
**This was a learing expreience for me in hosting a large interactive notebook on binder**

* To get it to work i had to do a few things:
- [X] First, I had to convert the .ipynb to .py using nb... then using pipreqs i generated a requirements.txt file that 
showed all the dependencies. This alone wasnt sufficient.
- [x] I had to use conda to created an environment an environment(prosper_env) `conda create -n env_name list of packages`, 
where i installed all the relevant packages, packages not found on conda were installed with pip
then I exported the environment using the code `conda prosper_env export > environment.yaml`
> to remove environment use `conda env remove -n env_name`

> Relevant links on udacity [here](https://classroom.udacity.com/nanodegrees/nd002/parts/6f1ba175-1429-48e9-ab26-44d08ab21e7e/modules/77f8d550-a127-4d89-ad83-a0d6a38cc3b8/lessons/902a64cd-8435-46f3-8c05-f8aae1ce8a3b/concepts/14783a82-d656-436b-bc3f-12f7abe03529), on binder
[here](https://mybinder.readthedocs.io/en/latest/tutorials/reproducibility.html), [here](https://mybinder.readthedocs.io/en/latest/sample_repos.html#python-environment-with-requirements-txt) and [here](https://mybinder.readthedocs.io/en/latest/sample_repos.html#python-environment-with-requirements-txt), on conda website
[here](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-non-conda-packages), on [medium](https://medium.com/@boscacci/why-and-how-to-make-a-requirements-txt-f329c685181e), on github [here](https://github.com/binder-examples/python-conda_pip/blob/master/environment.yml) and [here](https://github.com/bndr/pipreqs/issues/51) 
and finally on stackoverflow [here](https://stackoverflow.com/questions/31684375/automatically-create-requirements-txt)
