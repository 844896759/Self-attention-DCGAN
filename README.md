# Self-attention-DCGAN

***An application on the SAGAN from https://github.com/heykeetae/Self-Attention-GAN. I re-constructed part of code and added a 28 by 28 version running on mnist dataset.***

### Core files for running the code:

1. SAGAN_mnist.ipynb: A notebook interface containing codes for loading mnist dataset, utility functions and training function.

2. model_28.py: Contains self-attention, Generator and Discriminator modules for 28 by 28 version.

3. spectral.py: Containing spectral normalization module. Borrowed from https://github.com/heykeetae/Self-Attention-GAN. Can be removed given minor change in model.py.

4. download_dogs.sh: Bash script for downloading the dog dataset from http://vision.stanford.edu/aditya86/ImageNetDogs/.

### Model Structure:

![model_structure](demo/model_structure.png)

### Deep Convolutional GAN VS Self Attention GAN

![comparison on mnist](demo/comparison_mnist.gif)

![comparison on celebA](demo/comparison_celebA.gif)

### Referance:

[1] Han Zhang, Ian Goodfellow, Dimitris Metaxas, Augustus Odena: “Self-Attention Generative Adversarial Networks”, 2018;

Full paper: https://arxiv.org/pdf/1805.08318.pdf

[2] Xiaolong Wang, Ross Girshick, Abhinav Gupta, Kaiming He: “Non-local Neural Networks”, 2017; 

Full paper: https://arxiv.org/pdf/1711.07971.pdf

[3] Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Lukasz Kaiser, Illia Polosukhin: “Attention Is All You Need”, 2017;

Full paper: https://arxiv.org/pdf/1706.03762.pdf
