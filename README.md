# INM702_Coursework - Aaron Mir
Task 1: Pathfinding Game, Task 2: Classification of MNIST, Task 3: Comparison with PyTorch

File name: T1Aaron_Mir_INM702_Task_1

A pathfinding game which uses an Agent in a Maze to find the shortest path from the top-left cell to the bottom right-cell of a 2D array where each element in this array represents the time an agent spends in the cell. Algorithms implemented include a Naive approach based on recursion, ant-colony optimisation and Dijkstra's algorithm for finding the shortest path. In the zip file, there are .png files demonstrating examples of paths found by the agent. The working out for dijkstra's implementation can be seen in the dijkstramain.ipynb file and likewise for antcolmain.ipynb. These are not important files but demonstrate the working out required to implement the algorithms.

To run this task, just run the Agent class cell, the IntMaze class cell and then depending on what algorithm you would like to test, you choose from the next 3 cells. You can modify the height and width of the maze, the name of the Agent and which algorithm you wish to run. For ant-colony optimisation, the input parameters of the start_game method correspond to the number of iterations, number of ants, alpha, beta and rho (pheromone evaporation rate) respectively. I have put default values in there.

At the output, the shortest path is shown on a graph of nodes which contain vectors showing the direction of the path. Note: Maze size should be NxN in order for the graph to show up properly.

File name: T2Aaron_Mir_INM702_Task_2

A neural network for the classification of the MNIST dataset. The model uses fully-connected layers, sigmoid, relu and softmax activation functions and categorical cross-entropy loss. The optimiser of choice was Adam. The outputs of the file are: training accuracy/loss curves, overall training accuracy and loss and the testing accuracy and loss. This was done for both fully sigmoid and fully relu hidden layer activation in order to compare the two approaches. In both cases, the output layer activation function was softmax and the loss was calculated using categorical cross-entropy.

In order to run the task, simply run the cells up until the end of the Neural Network (fully Sigmoid) section. The first block of cells are preprocessing of the MNIST dataset which involves loading, normalising, centering, standardising, flattening and shuffling the training and testing data. After that, there are classes to represent the different objects in the neural network. Once those were initialised, fully relu and fully sigmoid neural networks were explored and the results can be seen at the outputs.

The working out/testing of all the classes was conducted on a seperate dataset in the (Class Testing Area) at the bottom of the .ipynb file (after the end of the Neural Network (fully Sigmoid) section). This is not an important part of the code to view.

File name: T3Aaron_Mir_INM702_Task_3
This file contains the same neural networks as in Task 2 for the classification of the MNIST dataset but instead using PyTorch. The evaluation metrics for the neural networks designed in Task 2 were compared with the evaluation metrics for the neural networks designed in this task. In addition, a convolutional neural network was designed in PyTorch to demonstrate the effectiveness of convolutional layers in the classification of the MNIST dataset. The CNN achieved an accuracy of 0.988.

To run the task, simply run the cells and the outputs and evaluation metrics will be in the output.
