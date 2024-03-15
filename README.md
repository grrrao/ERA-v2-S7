# Overview of explorations and model results:

### Model 1. (1-4) Skeleton, BN
1. start with base model
   - 11k parameters, 
   - 99.45% training, 
   - 99.1% testing, 
   - so overfitting. 
2. changed to 10 channels (latest file)
    - 8.9k parameters.
    - 99.27 training. 
    - 99.05 testing
    - some overfitting. 


### Model 2. (5-8) Regularization, Dropout, GAP, Capacity, MP location
1. basing it on 10 channels as in model 1:
    - 4.9k parameters
    - 98.67 training
    - 98.90 testing
    - some underfitting

2. Added MP at output of 8, removed last convolution
    - 3.9k parameters
    - 98.05 training
    - 99.05 testing
    - some underfitting

      
### Model 3. (9-10) Image Augmentation, Learning Rates
1. basing on channels from model 2:
    - 3.9 k parameters
    - 97.6 training
    - 98.7 testing
    - still underfitting
2. bumping up to 16 channels to increase parameters
    - 6.6k parameters
    - 98.42 training
    - 99.15 testing
3. moving MP above GAP
    - 6.6k parameters
    - 98.6 training
    - 99.2 testing
4. increasing 16 to 24 in a layer. 
    - 7.8k parameters
    - 98.5 training
    - 99.3 testing
