# Apply an animated style to Images using GAN and White-box Representation

- Tensorflow implementation for paper “Apply an animated style to Images using GAN and White-box Representation”.
- All the documentation and paper is accessible from: https://drive.google.com/drive/folders/103JDFRrsvWfuUhWAL3VVULPS78AywfQK?usp=share_link

<img src="images/method.jpg" width="1000px"/>
<img src="images/use_cases.jpg" width="1000px"/>

## Use cases

### Scenery
<img src="images/city1.jpg" width="1000px"/>
<img src="images/city2.jpg" width="1000px"/>

### Food
<img src="images/food.jpg" width="1000px"/>

### Indoor Scenes
<img src="images/home.jpg" width="1000px"/>

### People
<img src="images/person1.jpg" width="1000px"/>
<img src="images/person2.jpg" width="1000px"/>


## Prerequisites

- Training code: Linux or Windows
- NVIDIA GPU + CUDA CuDNN for performance
- Inference code: Linux, Windows and MacOS


## How To Use

### Installation

- Assume you already have NVIDIA GPU and CUDA CuDNN installed 
- Install tensorflow-gpu 
- Install scikit-image==0.14.5, other versions may cause problems
- Install numpy==1.23.1, other versions may cause problems


### Inference with Pre-trained Model

- Store test images in /test_code/test_images
- Run /test_code/cartoonize.py
- Results will be saved in /test_code/cartoonized_images


### Train

- Place your training data in corresponding folders in /dataset 
- Run pretrain.py, results will be saved in /pretrain folder
- Run train.py, results will be saved in /train_cartoon folder
- Codes are cleaned from production environment and untested
- There may be minor problems but should be easy to resolve
- Pretrained VGG_19 model can be found at following url:
https://drive.google.com/file/d/1s7rLnubm25IpZEGUwRmR75kbTCUo3GfI/view?usp=share_link



### Datasets

- Dataset is accessible through the link:
  <br/>Raw:
  https://drive.google.com/drive/folders/1BnYlMiXqjDfXPmnH3dC1aKBy0q9Ytfuu?usp=share_link
  <br/><strong>Processed</strong>:
  https://drive.google.com/drive/folders/1BnYlMiXqjDfXPmnH3dC1aKBy0q9Ytfuu?usp=share_link
- Scenery images are collected from Shinkai Makoto, Miyazaki Hayao and Hosoda Mamoru films
- Clip films into frames and random crop and resize to 256x256
- Portrait images are from Kyoto animations and PA Works
- We use this repo(https://github.com/qhgz2013/anime-face-detector) to detect facial areas
- Manual data cleaning will greatly increace both datasets quality


## License
- Copyright (C) Xinrui Wang All rights reserved. Licensed under the CC BY-NC-SA 4.0 
- license (https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode).
- Commercial application is prohibited, please remain this license if you clone this repo
