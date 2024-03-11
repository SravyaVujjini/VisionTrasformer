# Implementation of an Efficient Vision Transformer

Implemented the base model of the Vision Transformer Architecture based on the research paper https://arxiv.org/pdf/2010.11929.pdf for the image classification purposes. 

## Architecture

![image](https://github.com/SravyaVujjini/VisionTransformer/assets/121740546/ba103744-e01c-4e57-8a80-74319ddba446)

The flowchart above depicts the architecture of the implemented ViT model.

### Input Processing

- Input images are divided into fixed-sized patches and treated as individual tokens which are flattened to 1D sequence and linearly projected to lower dimensional space.
- Below is an example of the input image divided into patches.
  
![image](https://github.com/SravyaVujjini/VisionTransformer/assets/121740546/a9b62f34-7bd4-4ea5-9d9d-34d25e0e50d4)

- Positional Encoding is applied to embedded patches, thereby capturing the spatial information of each patch

### Encoder Block

- Encoder block is the key component in transformer-based architecture, that performs self-attention, and captures complex features and dependencies from the input.
- The self-attention layer takes in the sequence of patch embeddings as input and computes a new set of embeddings by attending to all the other patches in the sequence
- This is followed by the feedforward layer which takes the attention output as the input and applies two linear transformations, followed by a non-linear activation function (ReLU)
  
### MLP Classifier

- The resulting sequence of patch embeddings is fed into a multi-layer perceptron (MLP) classifier which consists of one or more fully connected layers with the non-linear activation function GELU. 

![image](https://github.com/SravyaVujjini/VisionTransformer/assets/121740546/1d4407b1-e3cd-47ff-a9a6-ef86f4983e2c)

This base model implementation consists of 2 encoder blocks with approx. 2.5M parameters unlike the original ViT base implementation that contains 86M parameters.

- Key parameters used: Embed dimensions: 128, Hidden layers: 256, MLP heads: 4, patch size: 4.

## Results

![image](https://github.com/SravyaVujjini/Image-Classification-using-ViT/assets/121740546/42b9d912-be76-4a24-b823-c4463dbc17d3)

![image](https://github.com/SravyaVujjini/VisionTransformer/assets/121740546/0575b310-3df8-45b0-aec1-b99b44f175ba)




