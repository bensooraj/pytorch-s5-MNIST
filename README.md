# PyTorch MNIST Dataset Deep Learning Experiment

## 1. Introduction
This project demonstrates the use of,
1. PyTorch to write neural networks
2. MNIST dataset for image classification and
3. Metal Performance Shaders (MPS) backend for GPU training acceleration (on Mac computers with Apple silicon)

## 2. Project structure
This project is organised as shown below,
```sh
.
├── Makefile    # Common maintenance scripts
├── README.md   # What you are reading now
├── S5.ipynb    # Jupyter Notebook that we will launch in a bit
├── model.py    # The two neural network models are defined in this file
└── utils.py    # Helper functions for training and testing the model

1 directory, 5 files
```

## 3. How to run 
1. Make sure `JupyterLab` is installed,
```sh
$ jupyter --version
Selected Jupyter core packages...
IPython          : 8.19.0
ipykernel        : 6.28.0
ipywidgets       : not installed
jupyter_client   : 8.6.0
jupyter_core     : 5.5.1
jupyter_server   : 2.12.1
jupyterlab       : 4.0.9
nbclient         : 0.9.0
nbconvert        : 7.13.1
nbformat         : 5.9.2
notebook         : not installed
qtconsole        : not installed
traitlets        : 5.14.0
```

If not, install it,
```sh
# Using pip:
$ pip install jupyterlab
# OR using Homebrew, a package manager for macOS and Linux
$ brew install jupyterlab
```

2. Clone this repository to your local machine.
```sh
$ git clone https://github.com/bensooraj/pytorch-s5-MNIST
$ cd pytorch-s5-MNIST
```

3. Start the lab!
```sh
$ make start-lab
```
This should automatically launch your default browser and open `http://localhost:8888/lab`.

All set!

## 4. Challenges
1. The MPS backend doesn't work properly `shuffle=True` for [`torch.utils.data.DataLoader`](https://pytorch.org/docs/stable/data.html#module-torch.utils.data).

## 5. Resources
1. [Accelerated PyTorch training on Mac](https://developer.apple.com/metal/pytorch/)
2. [PyTorch: MPS BACKEND](https://pytorch.org/docs/master/notes/mps.html)
3. [A Simple Conv2D Dimensions Calculator & Logger](https://charisoudis.com/blog/a-simple-conv2d-dimensions-calculator-logger)
