# Neural Networks

Jupyter notebooks for the Neural Networks course at Aristotle University of Thessaloniki (2024). Every task classifies the [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html) images (60,000 images, 10 classes) and compares the results with classical classifiers.

## Tasks

| Notebook | Topic |
|---|---|
| `task_0.ipynb` | 1-NN, 3-NN and Nearest Centroid baselines, with scaling, PCA and noise as preprocessing |
| `Task_1.ipynb` | MLPs (linear, ReLU, deeper, batch normalization with momentum, dropout) and CNNs in PyTorch |
| `Task2.ipynb` | SVMs with linear, RBF and polynomial kernels, hyperparameter search and bagging |
| `Task3.ipynb` | RBF neural networks with random and k-means centres, fixed and trainable |

Each notebook explains every step and ends with a comparison against the earlier models.

`Ex1_Models/` holds the trained weights from Task 1, so the models can be loaded without retraining.

## Setup

1. Download the **CIFAR-10 python version** from https://www.cs.toronto.edu/~kriz/cifar.html.
2. Extract it and copy `data_batch_1` … `data_batch_5`, `test_batch` and `batches.meta` into the repository folder. The notebooks read them from there. The dataset is not stored in this repo.
3. Install the dependencies:

   ```bash
   pip install numpy pandas matplotlib scikit-learn torch torchmetrics mlxtend jupyter
   ```

4. Run `jupyter notebook` and open a notebook.

A GPU is used automatically if one is available.
