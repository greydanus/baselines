# Baselines
Sam Greydanus. 2018. MIT License.

_Written in PyTorch_

About
--------
A set of self-contained Jupyter notebooks aimed at providing quick and easy-to-modify baselines. Specifically:
 * [mnist-np]() a 3-layer dense relu network implemented entirely in NumPy (test acc: 96.8%)
 * [mnist-fc]() a 3-layer dense relu network implemented entirely in NumPy (test acc: 96.8%)
 * [mnist-cnn]() a 3-layer cnn relu network implemented entirely in NumPy (test acc: 98.7%)
 * [mnist-seq]() a 3-layer dense recurrent (GRU) network implemented on a sequentual MNIST task

I only trained these models on 1-3 epochs of MNIST, so they could probably do a little better. I wanted these baselines to be:
 * something I could train in ~2 minutes on my laptop
 * something that captured the general idea (of backprop, of neural nets, of cnns, of seq2seq models respectively)
 * something very reproducible (I save training stats and models along the way, etc.)
 * something easy to visualize/understand
 	* The code is minimal
 	* I plot training stats and a few examples at the end
 	* Each notebook is self-contained (minimal dependencies)

-> I don't include pretrained models for the MNIST baselines because each notebook runs in <5 minutes on a 2014 MacBook.
  
Dependencies
--------
* All code is written in Python 3.6. You will need:
 * NumPy
 * Matplotlib
 * [PyTorch 0.3$^+$](http://pytorch.org/): easier to write and debug than TensorFlow :)
 * [Jupyter](https://jupyter.org/)
 * maybe my [Excitation Backprop code](https://github.com/greydanus/excitationbp)

Pretty Plots
---------

Pure numpy classifier

![mnist-np-stats.png](static/mnist-np-stats.png)

Dense classifier (PyTorch)

![mnist-fc-stats.png](static/mnist-fc-stats.png)

Convolutional classifier (PyTorch)

![mnist-cnn-stats.png](static/mnist-cnn-stats.png)

Sequential Model (PyTorch)

![mnist-seq-stats.png](static/mnist-seq-stats.png)

