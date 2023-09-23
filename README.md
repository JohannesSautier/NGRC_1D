# 1D NGRC
The experiments apply parallel Next Generation Reservoir Computing (NG RC) to predict the evolution of the 1D Kuramoto-Sivashinsky equation. The input variables are divided into different groups according to their spatial location. The input states of each group are predicted in parallel with a single Reservoir Computer.

## Setup
The Conda virtual environment was set up with the following installations:
-Python 3.10.9
-Numpy 1.23.5
-Matplotlib 3.6.2
-Scipy 1.9.3

## Parallel architectures
The Multiprocessing tool is used to process tasks in parallel. In particular, the one step prediction of a specific spatial region is parallelized.

## Datasets
The training and test datasets of the KS equation are generated using the code provided by Vlachas et al.. The code can be found in the GitHub repo: https://github.com/pvlachas/RNN-RC-Chaos

## Quick Start 
1. Generate the training and testing data using the referenced Github repository
2. Save “testing_data_N100000.pickle” and “training_data_N100000.pickle” to the desired location
3. Update the testing and training data path in the main file to access the data
4. Set up the virtual environment
5. Run the main file
6. The main file will predict the evolution of the KS equation, perform a specific experiment and print a graphical interpretation of the results:
![prediction_Noise2 0961,Ridge para0 035098,k3,Groups512,Interaction25,Pred_lengh400,ltraining99997,ic_index3,Model Auto_contour](https://github.com/JohannesSautier/1D_NGRC/assets/114988239/6ef6cd8a-1c5c-42b8-8175-5a357fa62b78)


