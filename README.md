The main goal of the project is to apply computer vision algorithms covered in the course to 
solve a real-world problem such as facial detection , recognition and pose estimation.  
Task 1  
Use Viola-Jones algorithm for face detection. You have to understand how the algorithm 
uses a cascade of Haar Feature classifier to detect the face. Use the OpenCV 
implementation discuss the effect of changing the algorithm parameters. To eliminate false 
positive detection, you have to use skin detector to verify that the detected face.   
Task 2  
Detect facial landmarks which are well-defined points around the main face parts mouth 
nose eyes. It used for multiple purposes such as face alignment. Find and use a simple 
facial landmark detection to detect facial landmark discuss how the algorithm works.  
Task 3 
Use descriptor to get distinctive vector around each landmark. Concatenate all the 
landmarks vector to obtain a distinctive vector for the face. Use this vector to build a face 
verification on system. The system should take two facial images as an input and obtain the 
feature vector for each, then compare them to tell if the two facial images belong to the 
same subject. Try different matching techniques.  
Task 4 
Extend Task four to build Facial recognition system, build your own gallery you may use 
your faces and/or celebrities faces. Prob the system with image using the webcam and 
show wither the probed face is on the gallery and show nearest 3 matches
