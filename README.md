# MNIST_projects
There are four components to this project: the CNN model, the image processor, the natural language model, and the audio playback 

The CNN model has a standard architecture of Convolution Layer to Maxpooling Layer to Dropout before Flattening and moving unto the Fully Connected Layer. Data Augmentation was implemented through the ImageDataGenerator module from keras. The model consistently achieved around 93.5% accuracy on the test data, which is acceptable considering that no hyper-parameter tuning has taken place yet (there are plans for it). 
The image processor uses OpenCV to load images and convert them to grayscale before detecting the edges of the letters, fetching the contours, and forming boxes around the detected letters. These boxes are then used to form images which are passed onto the CNN model and classified. 
The audio playback is a simple Text-to-Speech module. 
The natural language model makes use of a library to detect correct words and then make changes based on Jaccard distance. It remains a work in process. 
