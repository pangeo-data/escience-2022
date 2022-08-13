# Setup: how to run the tutorial

This tutorial's goal is to provide a wide introduction to the Pangeo ecosystem. 
While participants will see all the core libraries and possibilities offered by the Pangeo software ecosystem, it is also important that they get some insights about what a Pangeo platform is and how to use it. 
This is why we put in place such a platform on top of EOSC federation thanks to provider CESNET. 
We recommend then running this tutorial using the EOSC/CESNET infrastructure, which is mainly a Dask-gateway enabled Jupyterhub offering some pre-cooked software environment. 
For more details on this deployment, you may want to take a look at [Daskhub helm chart](https://github.com/dask/helm-chart/tree/main/daskhub).

This pages will describe three ways of running the tutorial:

- Through the provided Pangeo platform deployed on EOSC resources (recommended)
- Locally on your personal computer
- Using various Binderhubs solutions


## Running the tutorial on the provided Pangeo platform

First, before the FOSS4G workshop, all the participants will have to create an EGI account and enroll to the Pangeo virtual organisation to have access to the platform.
There are only two simple steps to do:

1. Create an account on the development instance of EGI Check-In, clicking on: https://aai-dev.egi.eu/registry/co_petitions/start/coef:2. You can easily delegate authentication with academic or social account e.g. GitHub.
1. Enroll in the "vo.pangeo.eu" Virtual Organisation by clicking on: https://aai-dev.egi.eu/registry/co_petitions/start/coef:290.

It is important to perform these steps as early as possible in order for managers of the Virtual Organisation to approve your petition to join.

Once your enrollment to Pangeo VO has been validated, simply log out from EGI Check-in to refresh your account.

:::{note}
Before the start of the course, you need to register to the Pangeo EGI-ACE EOSC infrastructure.
:::

Then, you just need to click on [this link](https://pangeo-foss4g.vm.fedcloud.eu/jupyterhub/hub/user-redirect/git-pull?repo=https%3A//github.com/pangeo-data/foss4g-2022&urlpath=lab/tree/foss4g-2022/tutorial/pangeo101/&branch=main) to open a Jupyterlab on the correct folder for the tutorial.

Under the hood, this will clone the https://github.com/pangeo-data/foss4g-2022 repository and put you in the correct folder for executing our tutorial.

From there, you can open and execute any notebooks used during the workshop, enjoy!

Alternatively, you can also open notebooks one by one from the PANGEO 101 section of this Jupyterbook by clicking on the rocket icon 🚀 on top of the notebook and choosing Jupyterhub option.

:::{note}
After the FOSS4G workshop, you can continue to use the resources, but note that we would probably modify the service and things might not work from time to time. 
We would appreciate you get in touch with us to give us some feedback and be informed of the platform evolution. You can do this through [Github Discussions](https://github.com/pangeo-data/foss4g-2022/discussions).

You can also contribtue to "the Pangeo show and tell" online meetups.
:::


## Running on your own computer

Most parts of this tutorial were designed to run with limited computer resources, so it is possible to run on your laptop.
It is a bit more complicated as you will have to install the software environment yourself. Also ypu will not be able to test real cloud distributed processing with Dask gateway.

Steps to run this tutorial on your own computer are listed below and demonstrated _through Linux commands only_:

1. git clone the foss4g-2022 repository.
```bash
git clone https://github.com/pangeo-data/foss4g-2022.git
```
2. Install the required software environment with Conda. If you do not have Conda, install it by following these instructions (see [here](https://docs.conda.io/en/latest/miniconda.html)). Then create the environment, this can take a few minutes.
```bash
conda env create -n pangeo-foss4g -f foss4g-2022/.binder/environment.yml
```
3. Launch a Jupyterlab notebook server from this environment.
```bash
conda activate pangeo-foss4g
jupyter lab
```
4. Open a web browser and connect to the Jupyterlab provided URL (you should see it in the jupyter lab command outputs), something like: http://localhost:8888/lab?token=42fac6733c6854578b981bca3abf5152.
5. Navigate to foss4g-2022/tutorial/pangeo101/ using the file browser on the left side of the Jupyterlab screen.


## Running using a Binderhub deployment

[Binderhub](https://binderhub.readthedocs.io/en/latest/) is a cloud service that allows users to share reproducible interactive computing environments from code repositories. It is generally used to enable other users to easily run your own code through Jupyter notebooks. 
It is a really cool service offered for free by several organisations (MyBinder through Jupyter, GESIS, etc.).

It is probably the easiest way to execute notebooks in this repository, as you only have to do one click to arrive in a Jupyterlab with all the necessary libraries.
However, the hardware resources you will be allowed to use are quite small, so you will not be able to grasp the full potential of the Pangeo software stack, and parts of the notebooks will be unavailable.

All the notebooks on the PANGEO 101 section, for example ["Handling multi-dimensional arrays with xarray"](../pangeo101/xarray_introduction.ipynb) have a rocket icon at the top, from which you can select the Binder button to just run this notebook on the [GESIS Binder service](https://notebooks.gesis.org/binder/).

Alternatively, you can also directly click on the below buttons:

GESIS:

[![Binder](https://mybinder.org/badge_logo.svg)](https://notebooks.gesis.org/binder/v2/gh/pangeo-data/foss4g-2022/HEAD)

MyBinder:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/pangeo-data/foss4g-2022/HEAD)

You will then have to navigate to the foss4g-2022/tutorial/pangeo101/ folder using the file browser on the left side of the Jupyterlab screen.
