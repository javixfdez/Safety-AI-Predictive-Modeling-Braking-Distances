# Safety-AI-Predictive-Modeling-Braking-Distances
### By Javier Fernández Ramos, María Ángeles Muñoz Juan-Dalac and Marta González Pérez
Multilayer Perceptron with SiLU activations architecture to predict braking distances using synthetic generated data


## Abstract

This project explores the ability of neural networks to learn and reproduce real-world scenarios using synthetic generated data. We designed three candidate datasets based on the UV index, compound
interest and braking distance, finally selecting the latter due to mathematical tractability. A dataset was generated from the braking distance equation and used to train a multilayer perceptron with SiLU
activations. The optimized and tested 32-8 neuron architecture achieved exceptional performance (R2 = 0.99, MAE = 0.92) and showed an incredible alignment with the analytical solution, confirming its
ability to approximate this physics non-linear problem. This project successfully demonstrated that a lightweight neural network can replicate the braking distance with remarkable accuracy, highlighting
the potential of machine learning as a reliable and efficient tool for modelling actual safety and applied systems.


## Methods

Starting with the design of the braking distance predictive framework, the code is structured to simulate, preprocess, and model vehicle stopping distances using machine learning. The overall
purpose is to approximate the physical braking distance equation through a neural network (MLP) and compare the learned approximation with the analytical solution.

The first part of the code focuses on data generation. A function is defined to calculate the total
braking distance based on the physical model. Random samples are generated for vehicle speed, tire-pavement friction coefficient, and driver reaction time, ensuring realistic values. The braking
distance is then computed for each sample, and the resulting dataset is stored for further use.

The second stage involves data splitting, where the dataset is divided into training, validation, and test
sets. This ensures that the model can be trained, tuned, and evaluated on separate partitions, preserving the integrity of performance assessment.
