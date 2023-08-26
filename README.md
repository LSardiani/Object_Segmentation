# Object_Segmentation
Project 3 Self-driving car 

Hello there!
This project was the third project (Project 3) from IndonesiaAI Computer Vision (CV) Bootcamp Batch 2.

We utilised the Cityscapes Dataset (https://www.cityscapes-dataset.com) from the IndonesiaAI Dashboard (https://drive.google.com/drive/folders/1O-6KLENO8HLCT7UgSs38As25c5ddFQGj?usp=drive_link).

# Background
Semantic segmentation → process of assigning each pixel of the received image into one of the predefined classes, which represent the segment labels of the images e.g. roads, cars, signs, traffic lights, or pedestrians → “pixel-wise classification”

The main benefit : situation understanding. 
→ used in many fields such as autonomous driving, robotics, medical images, satellite images, precision agriculture, and facial images as a first step to achieving visual perception.

“The more we perform semantic segmentation with a high accuracy and a short time, the more correctly the ego vehicle understands the surrounding environment and accordingly make the right decision every moment.”

Various CNN based networks are proposed for semantic segmentation: U-Net, FCN, SegNet, ENet etc.

Ref: T. Sugirtha and M. Sridevi, "Semantic Segmentation using Modified U-Net for Autonomous Driving," 2022 IEEE International IOT, Electronics and Mechatronics Conference (IEMTRONICS), Toronto, ON, Canada, 2022, pp. 1-7, doi: 10.1109/IEMTRONICS55184.2022.9795710; Sellat Q, Bisoy S, Priyadarshini R, Vidyarthi A, Kautish S, Barik RK. Intelligent Semantic Segmentation for Self-Driving Vehicles Using Deep Learning. Computational Intelligence and Neuroscience. 2022/01/17 2022;2022:6390260. doi:10.1155/2022/6390260

# Getting started
In this project, we downloaded Dataset from (https://drive.google.com/drive/folders/1O-6KLENO8HLCT7UgSs38As25c5ddFQGj?usp=drive_link).

There were 12 classes.

# Model
We utilised the UNet model to perform this project

![Unet](https://github.com/LSardiani/Object_Segmentation/assets/135226112/9d66a041-3b9a-4302-b90a-b6952b7e461b)

Optimizer: Adam

Loss: Sparse Categorical Crossentropy

Using four different experiments by hyper-tuned the parameters:
![Screen Shot 2023-08-26 at 12 54 06](https://github.com/LSardiani/Object_Segmentation/assets/135226112/db1b1c0d-4b1e-4a7c-bbe5-2644c894c9e6)


# Results

Training and Validation Curves, Comparison between four models

Unet Model 1

![Unet1](https://github.com/LSardiani/Object_Segmentation/assets/135226112/f6e930f0-f905-47cd-bb87-5c87ee9e5829)

Unet Model 2

![Unet2](https://github.com/LSardiani/Object_Segmentation/assets/135226112/2903c45b-a9d0-4552-8fbc-94f2a8e325dc)


Unet Model 3

![Unet3](https://github.com/LSardiani/Object_Segmentation/assets/135226112/95b7a0cd-9dce-4dfb-b3b7-9819064e911e)


Unet Model 4

![Unet4](https://github.com/LSardiani/Object_Segmentation/assets/135226112/5327511c-1143-4d0d-9de5-138578fd575c)


# Actual prediction

Unet Model 1

![Val1](https://github.com/LSardiani/Object_Segmentation/assets/135226112/8ae84114-17d7-4fd9-bfa1-c3ddc70a419c)


Unet Model 2

![Val2](https://github.com/LSardiani/Object_Segmentation/assets/135226112/96eea773-c5e3-45f7-9974-82cb781897e5)


Unet Model 3

![Val3](https://github.com/LSardiani/Object_Segmentation/assets/135226112/e0300ce8-9c42-4ee3-81f0-f02bf1a7c0f3)


Unet Model 4

![Val4](https://github.com/LSardiani/Object_Segmentation/assets/135226112/5b83077b-1fd7-46fa-b9cb-011ff1245809)


# Deployment 

Unet Model 1

![Test1](https://github.com/LSardiani/Object_Segmentation/assets/135226112/68fb3eb2-face-4e73-bb4e-b5f9d4476455)


Unet Model 2

![Test2](https://github.com/LSardiani/Object_Segmentation/assets/135226112/b1dcc037-abf0-45a6-b677-3cc58ad2fca1)


Unet Model 3

![Test3](https://github.com/LSardiani/Object_Segmentation/assets/135226112/32cacd00-8ecf-404b-ae3c-8b86df418cd7)


Unet Model 4

![Test4](https://github.com/LSardiani/Object_Segmentation/assets/135226112/9c26565b-df75-4811-8918-56f832dd7dac)


# Summary for the four models:

Accuracy and Loss

![Screen Shot 2023-08-26 at 13 07 59](https://github.com/LSardiani/Object_Segmentation/assets/135226112/f9948579-f686-4f35-b4e5-5f6c1ee41e93)


IoU and Dice score

![Screen Shot 2023-08-26 at 13 28 36](https://github.com/LSardiani/Object_Segmentation/assets/135226112/d20caba3-51cb-4f79-a8b2-906a7ea6aab6)


# Conclusions: 
The Unet Model 3 gave the best model: image size 192, 256, epoch 150, buffer size 150, batch size 2.

# Contact
Please reach me by email: lilysilva.dr@gmail.com for any further discussion.

Thank you!
