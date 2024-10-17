# lightning-ai-demonstration

A quick and simple introduction to creating, training, and running a simple neural network to do image classification. It is presented [in Jupyter notebook form](https://github.com/merrillmckee/lightning-ai-demonstration/blob/main/src/lightning-ai-demo.ipynb) and can be shared in less than 60 minutes.

It leverages `Lightning` and `PyTorch`.

From `Lightning`, we inherit `LightningModule` which forms the basis for our neural network model. And we also use its `Trainer` to train our network. `Lightning` tries to build on top of `PyTorch` to simplify the process of building a neural network. Besides less code, this example could be run on a GPU (for example, I've done this with a Macbook Pro M2) with no code changes. The term GPU never appears in this notebook code; it has been abstracted away.

From `PyTorch`, we use the built-in MNIST dataset, we use its utilties to architect the fully connected neural network with 1 hidden layer, and we use its Adam optimizer. From its related libraries, `torchmetrics`, we track the network's training and validation accuracy.

Finally, outside of the notebook, we can optionally run `TensorBoard` to visualize the training progress with metrics.
