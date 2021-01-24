# Celebrity-Lookalike-Using-Computer-Vision
To achieve this, we will be using the face_recognition library, which is built using dlib’s state-of-the-art face recognition built with deep learning, is considered one of the simples libraries used for face recognition and manipulation. The model has an accuracy of 99.38% on the Labeled Faces in the Wild benchmark. With this library you can find faces, find and manipulate facial features, and identify faces in pictures. You can also use this library with other Python libraries to do real-time face recognition.

For more information on the face_recognition library, you can view their official page from here.
First, we create the directory structure where you would be uploading your photograph.
Now that we have successfully created the directory and uploaded your picture in that directory, we will start writing the code by importing the libraries that we will require during the course of this project.
 Create Function to Load Images and Face Encodings 
 What are Face Embeddings?
In 2015, researchers at Google introduced FaceNet. It is a deep neural network used for extracting features from an image of a person's face. FaceNet takes that image of the person's face as an input, and it gives vector of 128 numbers as an output. This output represent the most important features of that person's face. In machine learning, this vector is called embedding. The face_recognition library used in this project uses FaceNet to find out the face embeddings.
 Calculate Euclidean Distance 
 What is Euclidean Distance?
The Euclidean distance (also known as the Pythagorean distance) between two points in Euclidean space is the length of a line segment between those two points. It can be calculated from the Cartesian coordinates of the points using the Pythagorean theorem. Given below is the formula to calculate the Euclidean distance between 2 points in n-dimensional space:
Here, the face_distance() function compares a list of face encodings to a known face encoding and get a Euclidean distance for each comparison face. The distance tells you how similar the faces are.
Now we will load the image we uploaded from the local computer, and the folder containing the celebrity images using the load_images() function we created earlier.
Finally, in this step we will find the matching celebrity image against the image we uploaded from the local computer. This is what the final output will look like:
