# text-classification
ML implementations for autonomous classification of text answers from an NPS customer's survey.

The code is implemented in python3 using [Tensorflow](https://www.tensorflow.org) through [Keras](https://keras.io). [Scikit](https://scikit-learn.org) is used for metrics and cross-validation and [mpl pyplot](https://matplotlib.org/api/pyplot_api.html) for displaying results.

## Installation
It is expected to be used in a virtual environment, keeping all packages contained. To do so, clone the repository and run from a terminal:

`python3 -m venv ./venv`

If you change the path to the virtual environment (here expected to be *venv* inside the repository root), you must also replace the path used inside the notebooks (first code cell). More info on virtual environments [here](https://docs.python.org/3/library/venv.html).

Activate the virtual environment using `source venv/bin/activate`. Once inside the virtual environment, install the required packages using:

`pip install -r python-requirements`

## Running scripts
The scripts were implemented on [jupyter notebooks](https://jupyter.org). Run the jupyter server at the repository folder using `jupyter-notebook` inside the virtual environment.

Each notebook contains:

- *linear-regression*: Linear regression from a dictionary containing sentences as bag-of-words.
- *keras-bag of words*: Simple single full connected hidden layer with inputs as bag-of-words.
- *keras-word embedding-cnn-cross validation*: Processes sentences using word embedding, preserving its order, to be computed with convolutional neural networks taking advantage of this information. Applies hyper-parametrization through cross-validation.

Methods used here are nicely described in [this guide](https://realpython.com/python-keras-text-classification/#a-primer-on-deep-neural-networks).

