Kaggle house prices
====================================
Code supporting [Blog post about DVC](https://datacenternotes.com/2018/09/01/aws-server-less-data-pipelines-with-terraform-part-1/).


# Setup

## Python setup

Though not a requirement, we recommend using Anaconda to manage python dependencies. Here are the steps that we will walk you though:
- Setup Anaconda. 
- Setup conda environment
- Setup local env

### Setup Anaconda
To download Anaconda package manager, go to: <i>https://www.continuum.io/downloads</i>.

After installing locally the conda environment, proceed to setup this project environment.


### Setup local conda environment

For dependency management we are using conda-requirements.txt and requirements.txt. 
Please "cd" into the current reposotory and build your conda environment based on those conda-requirements and requirements:
 
```bash
conda create -n kaggle python=3.6
source activate kaggle
conda install -c conda-forge --file conda_requirements.txt
pip install -r pip_requirements.txt
```


To deactivate this specific virtual environment:
```bash
source deactivate
```

If you need to completely remove this conda env, you can use the following command:

```bash
conda env remove --name kaggle
```


# Authors/Contributors

See the list of [contributors](https://github.com/diogoaurelio/serverless-pipelines-blog-series/graphs/contributors) who participated in this project.
