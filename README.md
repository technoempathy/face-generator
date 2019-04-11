### Face Generator
# Train a deep convolutional GAN to generate new images

#### Generates new images based on a dataset of celebrity pictures.
## Getting Started
### Step 1: Review my code in [dlnd_face_generation.ipynb](https://github.com/technoempathy/face-generator/blob/master/dlnd_face_generation.ipynb "Title") and see my results in [bike_sharing.ipynb](https://github.com/technoempathy/bike_sharing/blob/master/bike_sharing.ipynb "Title").

### Step 2: Do this project yourself
To make your own Face Generator, go [here](https://github.com/udacity/deep-learning-v2-pytorch "Title") and clone the repository.
```
git clone https://github.com/udacity/deep-learning-v2-pytorch.git
cd deep-learning-v2-pytorch/project-face-generation
```
Then open dlnd_face_generation.ipynb. 

## Prerequisites
1. Jupyter Notebooks
2. GPU
3. The [CelebFaces Attributes Dataset (CelebA)](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html). 
4. PyTorch and Torchvision. For installation instructions see [Udacity's README in the Deep Learning repository](https://github.com/udacity/deep-learning-v2-pytorch "Title").

## Tips
#### Watch out for size mismatch. 
Almost all the challenges I ran into with this project happened as a result of size mismatch. Read the comments in my code to see where I had these problems and how I solved them.

## Known Issues
* CELEB(A) dataset is highly biased based on race and facial symetry. 
* This model should be trained for aproximately 7 epochs, rather than 10.
* Generator should drop lower; I a model wherein it, by incresing g_conv_dim to 128, reducing batch_size to 32, and using xavier-normal weight initalization, adding dropout to the discriminator, and activating label smoothing - however the quality of the generated images decreased.

## Authors
- @technoempathy – Layla Messner 

## Acknowledgments
-	@udacity for the project
-	@facebook for the scholarship to the Udacity Deep Learning Nanodegree
