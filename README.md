# SudokuSolver

## Description
This project solves a Sudoku puzzle and overlays the solution onto the image in real time. This project is based off of the project from geaxgx1 found here: https://www.youtube.com/watch?v=QR66rMS_ZfA 

## Method
In general Sudoku is solved using the Backtracking approach (bruteforce). Here we are using the Greedy Best First Search Approach algorithm. A modified version of the Naive Back Tracking method. IT selects the path which appears best at that moment. It is the combination of deapth-first search and breadth-first search algorithms. 
The greedy best first algorithm is implemented by the priority queue. Find more information about the method here: https://medium.com/@mygreatlearning/bfs-best-first-search-concept-algorithm-and-implementation-d5c5b1b6e4d
The strategy that I used is inspired by https://norvig.com/sudoku.html

## Steps
1. Reads image from real time input or a video or an image. 
2. Convers input image to black and white. Applies threshold to remove unwanted noise. 
3. Get the boundary of the largest countour. (the outline of the sudoku matrix)
4. In each cell of the sudoku matrix, detect if any number si there or not byfinding contours.
5. Predict those detected numbers. 
6. Input the predicted numbers into Sudoku SOlving algorithm and get the output. 
7. Overlay the corresponding calculated results on the live image/video.

## How to Run 
1. Install all required libraries in requirements.txt 
2. Directly run all cells of sudoku testing.py file. It does all the imports by itself. 
3. Grab your Sudoku puzzle in front of your camera and solution will be relayed over their respective questions.
4. To stop the camera, click 'Q" on keyboard.

## Additional Resources Used
https://medium.com/@o.kroeger/tensorflow-mnist-and-your-own-handwritten-digits-4d1cd32bbab4
https://maker.pro/raspberry-pi/tutorial/grid-detection-with-opencv-on-raspberry-pi
https://www.pyimagesearch.com/2014/05/05/building-pokedex-python-opencv-perspective-warping-step-5-6/
https://www.programcreek.com/python/example/89417/cv2.arcLength
https://csfieldguide.org.nz/en/interactives/pixel-viewer/
http://www.ee.surrey.ac.uk/CVSSP/demos/chars74k/
