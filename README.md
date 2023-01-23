# Neural_Network_Charity_Analysis
20: The Rise of Machine Learning

## Overview of the analysis

The aim of the analysis was to determine whether the applicants will be successful if funded by Alphabet Soup Charity. This was achieved by analysing the data using deep learning, specifically the neural network models accompanied with Tensorflow and Python.

## Resources 

  - Datasource: [charity_data.csv](https://raw.githubusercontent.com/fareenamughal/Neural_Network_Charity_Analysis/main/Starter_Code/charity_data.csv)
  
  - Software: Python 3.9.15, Anaconda and Jupyter Notebook

## Results

### [Images of the various optimazation results]

### Preprocessing of Data
- The EIN and NAME columns which are identifiers have been removed
- The features of the model are included as part of the columns listed below and the unique number of unique values in   each columm is also indicated
    - APPLICATION_TYPE            17
    - AFFILIATION                  6
    - CLASSIFICATION              71
    - USE_CASE                     5
    - ORGANIZATION                 4
    - STATUS                       2
    - INCOME_AMT                   9
    - SPECIAL_CONSIDERATIONS       2
    - ASK_AMT                   8747
    - IS_SUCCESSFUL               2
  
  - The target is the column - IS_SUCCESSFUL. This has the results which holds whether the findomh was used effectively. The results are indicated as a yes or no denoted by 1 or O.

### Compiling, Training and Evaluating the Model
1. Different options of hidden layers have been tested as well as number of nuerons
    - The model that gave the best results had 3 hidden layers with 90 and 30 neurons respectively.
2. Various activation functions were used including Tanh, ReLu and Sigmoid. 
    - The model with the best result used ReLu and Sigmoid activation 
3. Number of parameters tested for the model with the best results was 6,811
4. The efficiency of the model remained below 75%, if the callback function was applied this may have been achieved(tensorflow errors prevented me from trying this). To try and increase the results was difficult as I had already achieved the best result with my first try which resulted in a 72.29% efficiency.
5. So as to try and optimize the accuracy, I tried to change the following:
    - activation functions - this being a binary model worked best with ReLu and Sigmoid activation
    - number of hidden layers - the model worked with 2 hidden layer and the change to 5 or 3 hidden layers did not     
    - materially improve the results 
    - Epoch size - increasing this resulted in larger number of records but also increased processing time. 
    - The type of model used - Random classifier, also resulted in very similar results.  

## Recommendation



There is a bulleted list that answers all six questions (15 pt)
Summary:

There is a summary of the results (2 pt)
There is a recommendation on using a different model to solve the classification problem, and justification (3 pt)
