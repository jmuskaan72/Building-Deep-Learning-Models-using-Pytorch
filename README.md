# Building-Deep-Learning-Models-using-Pytorch
Introduction to deep learning using pytorch and better insights on some DL models.

This series will cover various topics on Deep Learning: building neural networks with PyTorch, image classification, CNNs, GANs etc. in a hands-on workshop format. 

I took help from Jovian community which is a great source to track & reproduce our data science projects, collaborate easily with friends & colleagues, and automate repetitive tasks in our day-to-day workflow.

[JOIN THERE COMMUNITY.](https://community.jovian.ml/c/deep-learning-with-pytorch)

# PyTorch: Zero to GANs 
## SYSTEM SETUP : 
This tutorial takes a code-first approach towards learning PyTorch, and you should try to follow along by running and experimenting with the code yourself. We'll use the [Anaconda distribution](https://jovian.ml/outlink?url=https%3A%2F%2Fwww.anaconda.com%2Fdistribution%2F) of Python to install libraries and manage virtual environments. For interactive coding and experimentation, we'll use Jupyter notebooks. All the tutorials in this series are available as [Jupyter notebooks](https://jovian.ml/outlink?url=https%3A%2F%2Fjupyter.org%2F) hosted on [Jovian.ml](https://www.jovian.ml/): a sharing and collaboration platform for Jupyter notebooks & machine learning experiments.

Jovian.ml makes it easy to share Jupyter notebooks on the cloud by running a single command directly within Jupyter. It also captures the Python environment and libraries required to run your notebook, so anyone (including you) can reproduce your work.

Here's what you need to do to get started:

1. Install Anaconda by following the [instructions given here](https://jovian.ml/outlink?url=https%3A%2F%2Fconda.io%2Fprojects%2Fconda%2Fen%2Flatest%2Fuser-guide%2Finstall%2Findex.html). You might also need to add Anaconda binaries to your system PATH to be able to run the conda command line tool.

2. Install the jovian Python library by the running the following command (without the $) on your Mac/Linux terminal or Windows command prompt:
```
$ pip install jovian --upgrade
```
3. Download the notebook for this tutorial using the jovian clone command:
```
$ jovian clone aakashns/01-pytorch-basics
```

(You can copy this command to clipboard by clicking the 'Clone' button at the top of this page on Jovian.ml)

Running the clone command creates a directory `01-pytorch-basics` containing a Jupyter notebook and an Anaconda environment file.
```
$ ls 01-pytorch-basics
01-pytorch-basics.ipynb  environment.yml
```
4. Now we can enter the directory and install the required Python libraries (Jupyter, PyTorch etc.) with a single command using jovian:
```
$ cd 01-pytorch-basics
$ jovian install
```
`jovian install` reads the `environment.yml` file, identifies the right dependencies for your operating system, creates a virtual environment with the given name (`01-pytorch-basics` by default) and installs all the required libraries inside the environment, to avoid modifying your system-wide installation of Python. It uses `conda` internally. If you face issues with `jovian install`, try running `conda env update` instead.

5. We can activate the virtual environment by running
```
$ conda activate 01-pytorch-basics
```
For older installations of `conda`, you might need to run the command: `source activate 01-pytorch-basics`.

6. Once the virtual environment is active, we can start Jupyter by running
```
$ jupyter notebook
```
You can now access Jupyter's web interface by clicking the link that shows up on the terminal or by visiting [http://localhost:8888](https://jovian.ml/outlink?url=http%3A%2F%2Flocalhost%3A8888) on your browser.

## What it includes:
1. PyTorch Basics: Tensors & Gradients
2. Linear Regression & Gradient Descent
3. Image Classfication using Logistic Regression
4. Training Deep Neural Networks on a GPU
5. Convolutional Neural Networks, Regularization and ResNets
6. Generative Adverserial Networks
