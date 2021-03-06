# Entry_Task_Sudoku
_this git repository contains code and dataset that are used to build a machine learning model.<br>
the model should detect and recognize Sudoku Puzzle from newspapers images and return the detected Sudoku in an array._
## Implementation Technique :

 _the implementation of this model is splitted into 2 parts_:
  - first : _various image processing techniques such as Hough Transform and Contour Detection are used to detect the grid and digits
  of the Sudoku puzzle_. 
  - second  :  _create **Convolutional Neural Networks CNN model**  using **Keras API** to recognize each digit_.

_the reason for choosing this techniques is :_
 - _to build a Tensorflow model from scratch to detect the whole sudoku puzzle directly is hard in our case because we need to label more images with diffrent font style and diffrent quality, because for such a task 200 images are not enough.that's why i have decided to do image processing first to detect cells and use **Keras** (which is also a **Tensorflow API**) to train a model that is able to recognize each digit_.<br>
<br>**Note**: _due to the already mentioned techniques of implementation i exported the model as '.h5' file format_.

_my implementation is based on the following research papers which have been published when creating the sudoku dataset used to train my model_ : 
 - <a href="https://www.researchgate.net/publication/282303748_Camera-based_Sudoku_recognition_with_deep_belief_network" rel="nofollow">Camera-based Sudoku recognition with deep belief network</a>
 -  <a href="https://www.researchgate.net/publication/307545305_Mixed_handwritten_and_printed_digit_recognition_in_Sudoku_with_Convolutional_Deep_Belief_Network" rel="nofollow">Mixed handwritten and printed digit recognition in Sudoku with Convolutional Deep Belief Network</a>
 <br>
 
##  Run Examples : 
 
   - _to test the trained model just execute the code in the **Test_sudoku_model.ipynb** jupyter notebook and follow the instructions mentioned in it._
   - _I have uploaded some sample images for testing (images are located in the **test_examples_images** directory), you can also test with different images just put them into this directory and make sure to give a correct path of the image to the function **split_test_image_puzzle**_.<br>

<br>

 ## Installation of python module dependencies: 
  <br> _the following python modules should be installed :_
   
 - pip install opencv-python .
 - pip install tensorflow.
 - pip install keras 
 - pip install pytesseract.
 - pip install scikit-image
