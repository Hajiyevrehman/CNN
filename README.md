# Convolutional Neural Networks with PyTorch

For this project, we're going to use one of the most popular deep learning frameworks: PyTorch, and build our way through Convolutional Neural Networks.

## What is PyTorch?

PyTorch is a system for executing dynamic computational graphs over Tensor objects that behave similarly to numpy ndarray. It comes with a powerful automatic differentiation engine that removes the need for manual back-propagation.

## Why?

- Our code will now run on GPUs! Much faster training. When using a framework like PyTorch or TensorFlow you can harness the power of the GPU for your own custom neural network architectures without having to write CUDA code directly (which is beyond the scope of this class).
- We want you to be ready to use one of these frameworks for your project so you can experiment more efficiently than if you were writing every feature you want to use by hand.
- We want you to stand on the shoulders of giants! TensorFlow and PyTorch are both excellent frameworks that will make your lives a lot easier, and now that you understand their guts, you are free to use them :)
- We want you to be exposed to the sort of deep learning code you might run into in academia or industry.

## PyTorch Versions

This notebook assumes that you are using **PyTorch version >=1.0**. In some of the previous versions (e.g. before 0.4), Tensors had to be wrapped in Variable objects to be used in autograd; however, Variables have now been deprecated. In addition, 1.0 also separates a Tensor's datatype from its device and uses numpy-style factories for constructing Tensors rather than directly invoking Tensor constructors.

**If you are running on DataHub, you shouldn't face any problem.**
You can also find the detailed PyTorch [API doc](http://pytorch.org/docs/stable/index.html) here. If you have other questions that are not addressed by the API docs, the [PyTorch forum](https://discuss.pytorch.org/) is a much better place to ask than StackOverflow.

## Table of Contents

This assignment has 5 parts. You will learn PyTorch on **three different levels of abstraction**, which will help you understand it better and prepare you for the final project.

1. Part I: Preparation - we will use the CIFAR-100 dataset.
2. Part II: Barebones PyTorch - **Abstraction level 1**, we will work directly with the lowest-level PyTorch Tensors.
3. Part III: PyTorch Module API - **Abstraction level 2**, we will use `nn.Module` to define arbitrary neural network architecture.
4. Part IV: PyTorch Sequential API - **Abstraction level 3**, we will use `nn.Sequential` to define a linear feed-forward network very conveniently.
5. Part V: ResNet10 Implementation - we will implement ResNet10 from scratch given the architecture details.

Here is a table of comparison:

| API           | Flexibility | Convenience |
|---------------|-------------|-------------|
| Barebone      | High        | Low         |
| `nn.Module`     | High        | Medium      |
| `nn.Sequential` | Low         | High        |

## Part I. Preparation

First, we load the CIFAR-100 dataset. This might take a couple of minutes the first time you do it, but the files should stay cached after that.

## Usage

To run this project, follow the steps below:

1. Clone the repository:
    ```bash
    git clone https://github.com/Hajiyevrehman/KNN.git
    cd KNN
    ```

2. Ensure you have the necessary dependencies installed. You can install them using pip:
    ```bash
    pip install torch torchvision numpy
    ```

3. Follow the notebook or script instructions to run each part of the assignment.

## Conclusion

This project is designed to help you understand the different levels of abstraction in PyTorch and how to implement convolutional neural networks efficiently. By the end of this assignment, you should be comfortable with building, training, and evaluating deep learning models using PyTorch.

For more information, refer to the official PyTorch documentation [here](http://pytorch.org/docs/stable/index.html).
