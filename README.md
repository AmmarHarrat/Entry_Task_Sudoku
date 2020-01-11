# Entry_Task_Sudoku
_this git repository contains code and datasets that are used to build a machine learning model.
the model should detect and recognize Sudoku Puzzle from newspapers images and return the detected Sudoku in an array._
## Implementation Technique 

 _the implementation of this model is splitted into 2 parts_:
  - first : _various image processing techniques such as Hough Transform and Contour Detection are used to detect the grid and digits
  of the Sudoku puzzle_. 
  - second  :  _create **Convolutional Neural Networks model CNN** model using **Keras API** to recognize each digit_.

_the reason for choosing this techniques is :_
 - to build a Tensorflow model from scratch to detect the values of the whole sudoku puzzle directly is hard in our case because we need to label more images with diffrent font style and diffrent quality, because for such a task 200 images are not enough. 
 
