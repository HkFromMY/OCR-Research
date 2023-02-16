# OCR-Research
This repository is used to learn about Optical Character Recognition (OCR) and build a model with TensorFlow from scratch.

### Dataset used:
1. IAM Handwriting Images (https://fki.tic.heia-fr.ch/databases/iam-handwriting-database)
2. Synthetic Word 90K (https://www.robots.ox.ac.uk/~vgg/data/text/) (dataset used in this example)

### Credits:
1. https://github.com/VMD7/Automate-identification-and-recognition-of-handwritten-text-from-an-image
2. An End-to-End Trainable Neural Network for Image-based Sequence Recognition and Its Application to Scene Text Recognition by Baoguang Shi, Xiang Bai and Cong Yao School of Electronic Information and Communications Huazhong University of Science and Technology, Wuhan, China

### Steps to load weights

![image](https://user-images.githubusercontent.com/48499555/219261137-c158c9f4-81a7-4299-9057-d543bf5fbdc3.png)

### Limitation:

1. As this is a word-based predictor, which means the performance of this model depends on the segmentation techniques used for the image pre-processing steps. As shown above, the image segmentation fails to segments image in correct manner when single word image is fed into the system. 
2. Besides, the model also fails to predict when there are combination of digits and alphabets in the image as shown in the first example. This can be addressed by adding more samples data so that the model can extract useful pattern on this aspect.
3. The model can't also handle punctuation as this model is trained with synthetic word 90K dataset which does not have realistic english sentences which consists of alphabets, digits, and punctuations (including spaces).
