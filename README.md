# Implementation of an Efficient Vision Transformer

Implemented the base model of the Vision Transformer Architecture based on the research paper https://arxiv.org/pdf/2010.11929.pdf for the image classification purposes. 

## Architecture

![image](https://github.com/SravyaVujjini/VisionTransformer/assets/121740546/ba103744-e01c-4e57-8a80-74319ddba446)

The flowchart above depicts the architecture of the implemented ViT model.

### Input Processing

- Input images are divided into fixed-sized patches and treated as individual tokens which are flattened to 1D sequence and linearly projected to lower dimensional space.
- Below is the example of an input image divided into patches.
![image](https://github.com/SravyaVujjini/VisionTransformer/assets/121740546/a9b62f34-7bd4-4ea5-9d9d-34d25e0e50d4)


