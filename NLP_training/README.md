[![License](http://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](LICENSE.md)

## Prepare environment ##
Download anaconda for python3.6 from https://www.anaconda.com/distribution/ (request secure access if you are not able to install anaconda)

### Run commands ###

    See all the enviornments
    $ conda env list

    Create conda env
    $ conda create -n nlpenv python=3.6.6

    Activate the env
    $ conda activate nlpenv

    List all the installed packages
    $ conda list

    Change ENV variables
    $ cd %CONDA_PREFIX%
    $ mkdir .\etc\conda\activate.d
    $ mkdir .\etc\conda\deactivate.d
    $ type NUL > .\etc\conda\activate.d\env_vars.bat
    $ type NUL > .\etc\conda\deactivate.d\env_vars.bat

    Install all the necessary packages
    $ pip install -r requirements.txt

    Install spacy english library
    $ python -m spacy download en_core_web_sm
    
    Export the env in environment.yml file
    $ conda env export -n nlpenv -f environment.yml
    
    Run notebooks in jupyter-notebooks
    $ jupyter-notebook

    Deactivate env
    $ conda deactivate nlpenv

    Delete the env once done
    $ conda remove -n nlpenv --all
