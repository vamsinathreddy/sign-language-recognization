# sign-language-recognization
Firstly, install all necessary packages like OpenCV, Mediapipe, TensorFlow, etc. Using the OpenCV library, create a dataset of hand gestures corresponding to the letters of the alphabet and additional messages such as "thank you" and "nice to meet you." The data is captured using a webcam, and each gesture is associated with a specific class.

Next, the collected data is processed using the Mediapipe library for hand landmark detection. Landmarks are extracted from each frame to represent hand positions in the images, with 21 landmarks per hand (x, y coordinates).

The processed hand landmark data is then used to train a RandomForest classifier. The Pickle library is used to save and load data structures like dictionaries and models. The Numpy library is used for numerical operations. A RandomForest classifier is chosen for its high accuracy and efficiency compared to other algorithms like SVM and gradient boosting algorithms.

Using the Tkinter library, a GUI is created that provides real-time recognition of sign language through a live webcam feed. The recognized gestures are displayed as text on the screen. The system takes the most frequent character as input. Additionally, a spell checker module checks the spellings. If there is a 5-second gap, it treats the input as a word, and after an additional 5 seconds, it treats it as a sentence. The recognized text can then be converted into any language.
