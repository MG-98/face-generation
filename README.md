# Face generation by using GANs

# Introduction 
This is one of [Deep learning nanodegree](https://classroom.udacity.com/nanodegrees/nd101/parts/2e8d3b5d-aa70-4376-946f-0cdc37127d7d/modules/49d2e25d-6df2-48df-8ccd-88417ae208fc/lessons/368c9af3-c8b8-4b01-92ba-40d7e989d6e7/concepts/900d740a-e47d-4b67-be4c-ca27ea8981e2) major projects.
In this project, I have trained generative adversarial networks, especially [DCGAN](https://arxiv.org/pdf/1511.06434.pdf) to generate new images of faces.My goal was to get a generator network to generate new images of faces that look as realistic as possible!

# Dataset

I used  [CelebFaces Attributes Dataset (CelebA)](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) to train your adversarial networks.

# Trials 

- I have tried varuios moedel architicture :

    1- For model depth : [3 , 4] layers

    2- For convolution layer deimention : [32 , 64]

- I have tried also number of batch size : [32 , 64 , 128 ,256]

- I also have tried diffrient number of epochs : [ 20 , 30 , 50]

- As in the practise notebooks i used adam optimizer ,as it was recommended.

### The best model parameter 

Actually , the models has smal deffriences and can't appear from the few sample of photos i show , but we can deffirenciate between them by the loss perfornmence.As we can see in the above graphs , the best model with loss performence is the model with the following architicutre :

```python 
layer_in_depth = 4
conv_dim = 64
batch_size = 64
num_epochs = 10
```

To hava a closer look to the results of each model and its traing loss plot, i encourge you to have a look at the Training loss and generator sample of training in the following [report](https://github.com/MG-98/face-generation/blob/main/dlnd_face_generation.html)
