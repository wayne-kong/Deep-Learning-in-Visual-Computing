# ASU-Deep-Learning-Visual-Computing-CSE-598

Implementing Neural Networks from scratch using Python. The first 3 assignments included implementing neural networks with different architecture requirements, different activation and loss functions, dropout, batchnorm, and learning rate decay.<br>
The second 3 assignments included implementing different variations of CNN, GAN, and DANN using PyTorch.

# **DANN (Domain-Adversarial Neural Network) pytorch**

### Paper: [Domain-Adversarial Training of Neural Networks](https://arxiv.org/pdf/1505.07818.pdf)

<img src="/DANN.jpg" width="600" height="300" />


## **Prerequisite**

- python 3.7 (Anaconda)

- pytorch >= 1.0

- torchvision >= 0.2.2


## **Dataset**

- SVHN(Source dataset), MNIST(Target dataset)

- Download from torchvision

<p><img src="/svhn.jpg" width="300" height="300" /><img src="/mnist.jpg" width="300" height="300" /></p>


## **Description**

- DANN.ipynb : DANN model and training algorithm

- NN.ipynb : Baseline model and training algorithm to compare with DANN

- The models were trained by 20~30 epochs respectively

- You can see the graphs of loss and accuracy in ipynb


- **Implementation and Result**
>- GRL (Gradient Reversal Layer)
>- 3 Modules (Feature extractor, Classifier, Discriminator)
>- Data preprocessing (Resize 28x28, gray scale, normalization [-1, 1], )
>- 2 Datasets (SVHN, MNIST)
>- Test Accuracy (on MNIST test set)
>>- **DANN: 80.81 %**
>>- Baseline model (Source only model): 56.47 %

