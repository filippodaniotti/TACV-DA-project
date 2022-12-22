# Dataset

Both notebooks are compatible with ImageFolder style datasets, that follow this general rule

```
path_to_dataset/domain/class/image.extension
```

A more concrete example is such

```
dataset/mnist/0/img1.jpg
dataset/mnist/0/img2.jpg
dataset/mnist/0/img3.jpg
..
dataset/mnist/1/img1.jpg
dataset/mnist/1/img2.jpg
...
dataset/mnist/9/img100.jpg
dataset/mnist-m/0/img1.jpg
...
dataset/mnist-m/9/img100.jpg
```

We tested on Office31 and OfficeHome, both of which have this structure. For MNIST and MNIST-M we modified the structure of the dataset in order to match this style.

The notebook expects a compressed file containig the dataset that has to be specified in the initial configuration
