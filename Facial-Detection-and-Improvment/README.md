# Facial-Detection-and-Improvment

Our final project python code is the "final_project(group 81).ipynb" file.

Main idea: 
At first, we want to create a fully connected CNN(no FC layer at all), and then train this network on small images and set up CNN to output a 1x1x1 output. Then run the CNN on larger image, it will output the score for each box in the input image. However, we don't know how to create multi-dimensional labels (y), thus we used FC layers after CNN layers as instead. In this way, we can generate 1-D label very easy. So, following this idea, we begin to build our model as the following steps:

- step1: Transfer learning from well-known model (VGG-16), this could save our time to train model from scrach.
- step2: Add our own layers (FC layers) to VGG-16 and obtain our model.
- step3: Download human pictures and generate face images as part of training samples.
- step4: Training model

After model being built, we try to do:
- step1: Single face detection
- step2: Multi face detection

From the obtained results of singel/multi face dectection, we found our model is not accurate and efficient enough, thus we studied additional knowlege from Coursera deep learning course, and this course introduce YOLO model to us.
The first three sections(Build Model, Single Face Detection, Multi-Face Detection) are all finished by ourselves, the last part(YOLO) we did minor adjustment.

About reference:
Section Ⅰ (Build model), Ⅱ (Single Facial Detection), ⅡⅠ (Multi-Face Detection) are all finished by ourselves, without reference. Section Ⅳ is referenced from Coursera Deep Learning course, we made minor adjustment, we have already notice the code we wrote with comment.