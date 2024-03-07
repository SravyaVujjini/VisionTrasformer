# Implementation of an Efficient Vision Transformer

Implemented the base model of the Vision Transformer Architecture based on the research paper https://arxiv.org/pdf/2010.11929.pdf for the image classification purposes. 

## Architecture

![image](https://github.com/SravyaVujjini/VisionTransformer/assets/121740546/ba103744-e01c-4e57-8a80-74319ddba446)

The flowchart above depicts the architecture of the implemented ViT model.

### Input Processing

- The ViT model takes an input image of size H x W x C, where H and W are the height and width of the image, and C is the number of channels (typically 3 for RGB images and 1 for grayscale images).
- The image is divided into a grid of nonoverlapping patches, where each patch is of size P x P x C.
- The patch size P is a hyperparameter that can be tuned depending on the task and the size of the input image. Each patch is flattened into a vector of size P x P x C, which represents the features within that patch. 

