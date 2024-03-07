# Implementation of an Efficient Vision Transformer

Implemented the base model of the Vision Transformer Architecture based on the research paper https://arxiv.org/pdf/2010.11929.pdf for the image classification purposes. 

### Architecture

![image](https://github.com/SravyaVujjini/VisionTransformer/assets/121740546/ba103744-e01c-4e57-8a80-74319ddba446)



Vision Transformers (ViTs) have been the major focus in the field of computer vision, after they have demonstrated promising results in natural language processing. In this project, we have implemented a vision transformer using PyTorch for image classification, with a focus on efficiency and reduced complexity. The motivation behind ViTs is the need for object recognition models that can handle variable-sized inputs and model long-range dependencies. While CNNs have been successful in this field, we explored the potential of vision transformers and aimed to reduce their computational overhead. The focus of this project is towards the following research question: Can we reduce the complexity of the model while maintaining decent accuracy? Our base model consists of minimal encoder blocks and a reduced number of parameters, which enabled us to perform training using little computational complexity. We were able to achieve good results with just 15-20 training epochs. We tested our model on different types of classification tasks which includes datasets such as CIFAR10, MNIST, and Satellite Imagery. The performance of our base model on MNIST and Satellite Imagery have been significant with an accuracy of about 91% on MNIST and 85% on Satellite Imagery. Additionally, we performed hyperparameter tuning to further improve the efficiency of the base model. We further tried various techniques such as augmentation, etc. and commented a few findings regarding the same. In a nutshell, we have demonstrated that a simplified vision transformer can still achieve good results in image classification tasks for simpler datasets.
