# TensorFlow Tutorials

[Original repository on GitHub](https://github.com/abbasmalekpour/TensorFlow-DeepLearning)

Original author is [Abbas Malekpour]

## Introduction

* These tutorials are intended for beginners in Deep Learning and TensorFlow.
* Each tutorial covers a single topic.
* The source-code is well-documented.

## Tutorials

1. Simple Linear Model
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/01_Simple_Linear_Model.ipynb))

2. Convolutional Neural Network
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/02_Convolutional_Neural_Network.ipynb))

3. Pretty Tensor
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/03_PrettyTensor.ipynb))

3-B. Layers API
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/03B_Layers_API.ipynb))

3-C. Keras API
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/03C_Keras_API.ipynb))

4. Save & Restore
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/04_Save_Restore.ipynb))

5. Ensemble Learning
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/05_Ensemble_Learning.ipynb))

6. CIFAR-10
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/06_CIFAR-10.ipynb))

7. Inception Model
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/07_Inception_Model.ipynb))

8. Transfer Learning
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/08_Transfer_Learning.ipynb))

9. Video Data
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/09_Video_Data.ipynb))

10. Fine-Tuning
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/10_Fine-Tuning.ipynb))

11. Adversarial Examples
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/11_Adversarial_Examples.ipynb))

12. Adversarial Noise for MNIST
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/12_Adversarial_Noise_MNIST.ipynb))

13. Visual Analysis
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/13_Visual_Analysis.ipynb))

13-B. Visual Analysis for MNIST
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/13B_Visual_Analysis_MNIST.ipynb))

14. DeepDream
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/14_DeepDream.ipynb))

15. Style Transfer
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/15_Style_Transfer.ipynb))

16. Reinforcement Learning
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/16_Reinforcement_Learning.ipynb))

17. Estimator API
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/17_Estimator_API.ipynb))

18. TFRecords & Dataset API
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/18_TFRecords_Dataset_API.ipynb)) 

19. Hyper-Parameter Optimization
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/19_Hyper-Parameters.ipynb)) 

20. Natural Language Processing
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/20_Natural_Language_Processing.ipynb)) 

21. Machine Translation
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/21_Machine_Translation.ipynb))

22. Image Captioning
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/22_Image_Captioning.ipynb))

23. Time-Series Prediction
([Notebook](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/23_Time-Series-Prediction.ipynb))


## Obsolete Tutorials

Some of these tutorials use an API called PrettyTensor for creating
Neural Networks in TensorFlow, but the PrettyTensor API is now obsolete.
Some of the Notebooks are therefore also obsolete and they are clearly
marked at the top of each Notebook. It is recommended that you
instead use the Keras API for creating Neural Networks in TensorFlow.


## Forks

See the [selected list of forks](forks.md) for community modifications to these tutorials.

## Installation

There are different ways of installing and running TensorFlow. This section describes how I did it
for these tutorials. You may want to do it differently and you can search the internet for instructions.

If you are new to using Python and Linux then this may be challenging
to get working and you may need to do internet searches for error-messages, etc.
It will get easier with practice. You can also run the tutorials without installing
anything by using Google Colab, see further below.

Some of the Python Notebooks use source-code located in different files to allow for easy re-use
across multiple tutorials. It is therefore recommended that you download the whole repository
from GitHub, instead of just downloading the individual Python Notebooks.

### Git

The easiest way to download and install these tutorials is by using git from the command-line:

    git clone https://github.com/abbasmalekpour/TensorFlow-DeepLearning.git

This will create the directory `TensorFlow-Tutorials` and download all the files to it.

This also makes it easy to update the tutorials, simply by executing this command inside that directory:

    git pull

### Download Zip-File

You can also [download](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/archive/master.zip)
the contents of the GitHub repository as a Zip-file and extract it manually.

### Environment

I use [Anaconda](https://www.continuum.io/downloads) because it comes with many Python
packages already installed and it is easy to work with. After installing Anaconda,
you should create a [conda environment](http://conda.pydata.org/docs/using/envs.html)
so you do not destroy your main installation in case you make a mistake somewhere:

    conda create --name tf python=3

When Python gets updated to a new version, it takes a while before TensorFlow also
uses the new Python version. So if the TensorFlow installation fails, then you may
have to specify an older Python version for your new environment, such as: 

    conda create --name tf python=3.6

Now you can switch to the new environment by running the following (on Linux):

    source activate tf

### Required Packages

The tutorials require several Python packages to be installed. The packages are listed in
[requirements.txt](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/requirements.txt)
First you need to edit this file and select whether you want to install the CPU or GPU
version of TensorFlow.

To install the required Python packages and dependencies you first have to activate the
conda-environment as described above, and then you run the following command
in a terminal:

    pip install -r requirements.txt

Note that the GPU-version of TensorFlow also requires the installation of various
NVIDIA drivers, which is not described here.

### Python Version 3.5 or Later

These tutorials were developed on Linux using **Python 3.5 / 3.6** (the [Anaconda](https://www.continuum.io/downloads) distribution) and [PyCharm](https://www.jetbrains.com/pycharm/).

There are reports that Python 2.7 gives error messages with these tutorials. Please make sure you are using **Python 3.5** or later!

## How To Run

If you have followed the above installation instructions, you should
now be able to run the tutorials in the Python Notebooks:

    cd ~/development/TensorFlow-Tutorials/  # Your installation directory.
    jupyter notebook

This should start a web-browser that shows the list of tutorials. Click on a tutorial to load it.

### Run in Google Colab

If you do not want to install anything on your own computer, then the Notebooks
can be viewed, edited and run entirely on the internet by using
[Google Colab](https://colab.research.google.com). There is a
You click the "Google Colab"-link next to each tutorial listed above.
You can view the Notebook on Colab but in order to run it you need to login using
your Google account.
Then you need to execute the following commands at the top of the Notebook,
which clones the contents of this repository to your work-directory on Colab.

    import os
    work_dir = "/content/TensorFlow-Tutorials/"
    if os.getcwd() != work_dir:
        !git clone https://github.com/abbasmalekpour/TensorFlow-DeepLearning.git
    os.chdir(work_dir)

All required packages should already be installed on Colab, otherwise you
can run the following command:

    !pip install -r requirements.txt


## License (MIT)

These tutorials and source-code are published under the [MIT License](https://github.com/abbasmalekpour/TensorFlow-DeepLearning/blob/master/LICENSE)
which allows very broad use for both academic and commercial purposes.

A few of the images used for demonstration purposes may be under copyright. These images are included under the "fair usage" laws.

You are very welcome to modify these tutorials and use them in your own projects.
Please keep a link to the [original repository](https://github.com/abbasmalekpour/TensorFlow-DeepLearning).
