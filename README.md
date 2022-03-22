# Face-and-Eyes-Detection
## A simple face and eye detection model

![Ekran Alıntısı2](https://user-images.githubusercontent.com/48343735/159574769-6849d410-52ce-4ff9-b676-35d5223aef03.PNG)

How to Perform Face Detection with Deep Learning
by Jason Brownlee on June 3, 2019 in Deep Learning for Computer Vision
Tweet Tweet  Share
Last Updated on August 24, 2020

Face detection is a computer vision problem that involves finding faces in photos.

It is a trivial problem for humans to solve and has been solved reasonably well by classical feature-based techniques, such as the cascade classifier. More recently deep learning methods have achieved state-of-the-art results on standard benchmark face detection datasets. One example is the Multi-task Cascade Convolutional Neural Network, or MTCNN for short.

In this tutorial, you will discover how to perform face detection in Python using classical and deep learning models.

After completing this tutorial, you will know:

- Face detection is a non-trivial computer vision problem for identifying and localizing faces in images.
- Face detection can be performed using the classical feature-based cascade classifier using the OpenCV library.
- State-of-the-art face detection can be achieved using a Multi-task Cascade CNN via the MTCNN library.

## Face Detection
Face detection is a problem in computer vision of locating and localizing one or more faces in a photograph.

Locating a face in a photograph refers to finding the coordinate of the face in the image, whereas localization refers to demarcating the extent of the face, often via a bounding box around the face.

> A general statement of the problem can be defined as follows: Given a still or video image, detect and localize an unknown number (if any) of faces 

Detecting faces in a photograph is easily solved by humans, although has historically been challenging for computers given the dynamic nature of faces. For example, faces must be detected regardless of orientation or angle they are facing, light levels, clothing, accessories, hair color, facial hair, makeup, age, and so on.

> The human face is a dynamic object and has a high degree of variability in its appearance, which makes face detection a difficult problem in computer vision.

Given a photograph, a face detection system will output zero or more bounding boxes that contain faces. Detected faces can then be provided as input to a subsequent system, such as a face recognition system.

> Face detection is a necessary first-step in face recognition systems, with the purpose of localizing and extracting the face region from the background.

There are perhaps two main approaches to face recognition: feature-based methods that use hand-crafted filters to search for and detect faces, and image-based methods that learn holistically how to extract faces from the entire image.


