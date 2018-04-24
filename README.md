# Video_MotionDetection

I have  dataset of videos with walking and jogging  for video classification, created a 3-D CNN model  implemented in Keras .
I divide our approach into two parts :

 1 .Create video files into tensors and store in npy files:

1) Download dataset
2) Extract files and examine folder structure - each folder contains videos belonging to the category
3) Make data ready by generating a CSV file for training and testing, each CSV file containing path to video and category it belongs to.
4) Convert videos to numpy array files

2 . Define model load .npy files and train the model :

1) Load numpy files(train_data, train_labels,test_data,test_labels)
2) Pass them into Conv3D model written in Keras
3) Compile and observe results


It gave a testing accuracy of around 50% but greatly reduced time to train the model by already saving data in a numpy array.
Since the training data remains the same, there is no need to convert videos into numpy arrays every time we train the model.
