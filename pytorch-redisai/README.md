# Image Recognition with PyTorch and RedisAI - RedisConf Workshop

## Pre-Requisites

### Training Images for Transfer Learning
Prepare your own training set of images consisting of at least two classes (you can have more) with 30-50 images per class. You will train the neural network to recognize these from each other. For example, these could be dogs vs cats, two different models of cars, different types of flowers, or different types of anything.

If you don’t have your own sets, no worries, the instructor will give you a preselected training set.

### Setup

1. Create an account at https://kaggle.com/.
1. Install the Conda package manager locally: [https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html).
1. You may need to add the following environment variables:
    1. `export MINICONDA3_HOME=/$USER/miniconda3`
    1. `export PATH=$MINICONDA3_HOME/bin:$PATH`
1. Create and configure your local conda environment:
    1. `conda create -n py36_torch python=3.6`
    1. `source activate py36_torch`
    1. `conda install -y numpy scikit-learn pillow matplotlib jupyter`
    1. `conda install -c pytorch -y pytorch torchvision`
    1. `pip install ml2rt redisai python-twitter`
1. Install docker, [https://www.docker.com/get-started](https://www.docker.com/get-started).
1. Once docker is installed, run the following command line. It should start the Redis AI docker. It should say something like “Ready to accept connections” at the end of the init phase. If it does, everything is good.
    1. docker run -p 6379:6379 -it --rm redisai/redisai
1. All set!

### Notebooks 

The Live Coding notebooks that replicate the in-video steps are in the `live-coding` subfolder.
