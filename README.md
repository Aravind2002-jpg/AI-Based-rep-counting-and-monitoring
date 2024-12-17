**Description**

In this project, I designed an AI that uses webcam footage to accurately detect exercises in real time and counts reps. OpenCV is used to access the webcam on your machine, a pretrained CNN is implemented for real-time pose estimation, and custom deep learning models are built using TensorFlow/Keras to recognize what exercise is being performed. In addition, this project includes a guided data collection pipeline which is used to generate training data for the custom deep learning models. Using my data, the LSTM model achieved an accuracy score of 97.78% and a categorical cross-entropy loss of 1.51e-3 on the validation dataset. The attention-based LSTM achieved an accuracy score of 100% and a categorical cross-entropy loss of 2.08e-5 on the validation dataset. From that point, joint angles are extracted from the pose estimation coordinates and heuristics are used to track the exercise and count reps. Finally, visualization tools are included that display joint angles, rep counts, and probability distributions.

https://github.com/user-attachments/assets/62584040-fdc2-4779-875b-e5c7f219b1fc

**Features**

 - Implementation of Google MediaPipe's BlazePose model for real-time human pose estimation
 - Computer vision tools (i.e., OpenCV) for color conversion, detecting cameras, detecting camera properties, displaying images, and custom graphics/visualization
 - Inferred 3D joint angle computation according to relative coordinates of surrounding body landmarks
 - Guided training data generation
 - Data preprocessing and callback methods for efficient deep neural network training
 - Customizable LSTM and Attention-Based LSTM models
 - Real-time visualization of joint angles, rep counters, and probability distribution of exercise classification predictions
