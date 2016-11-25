# schibsted-study

## Preparing a Python environment with the scientific libraries

### Conda location install

Mind that it doesn't mess with your local `python`

 * Install http://conda.pydata.org/miniconda.html and then the required dependencies by doing:
`conda install jupyter scikit-learn pandas seaborn`.

 * Install tensorflow in the conda environment (see https://www.tensorflow.org/versions/r0.11/get_started/os_setup.html#anaconda-installation)

### Python virtualenv

For more experienced users:

 * http://virtualenvwrapper.readthedocs.org/ and https://pip.pypa.io/en/stable/ then:
 `pip install -r requirements.txt`

 * Install Tensorflow separately: https://www.tensorflow.org/versions/r0.11/get_started/os_setup.html#virtualenv-installation

### Dockerized option

```
docker pull twiecki/pydata-docker-jupyterhub
docker run -it -p 8888:8888 twiecki/pydata-docker-jupyterhub bash
cd ..; git clone https://github.com/pilipolio/schibsted-study.git; 
jupyter notebook --notebook-dir=./schibsted-study/notebooks --ip=* --no-browser
```

## Running a notebook

Go to the directoy `notebooks` and run `jupyter notebook` from here. It should directly open a browser tab where you can open each notebooks. 

