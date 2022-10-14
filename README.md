# Neural_Network_Charity_Analysis

## Overview
The purpose of this analysis was to use a Deep Learning Neural Network to help a firm decide which oirganization will recieve funding from donations based on the outcomes of previous organizations helped by AlphabetSoup over the last 20 years.

## Results 
- Data Preprocessing
  - What variable(s) are considered the target(s) for your model?
    - The target variable was the IS_SUCCESSFUL column which represented whether or not the organization which recieved a donation was successful 
  - What variable(s) are considered to be the features for your model?
    - The feature variables are listed in the image below: </br>
    ![This is an image](https://github.com/smwhng/Neural_Network_Charity_Analysis/blob/main/Images/features.PNG)
  - What variable(s) are neither targets nor features, and should be removed from the input data?
    - The variables EIN and NAME were identifiers for the various organizations and were neither targets nor features and were removed
  - In an attempt to remove noisy variables from some of the features, the APLICATION_TYPE and CLASSIFICATION variables were binned to group application types and classifications with less than 500 and 1000 values respectively as other. 
  - In addition, to try and increase the accuracy of the model, the INCOME_AMT variable was binned to group income amounts with less than 3000 values as other, the process for which can bee seen in the image below. </br>
  ![This is an image](https://github.com/smwhng/Neural_Network_Charity_Analysis/blob/main/Images/Noise%20post.PNG)
- Compiling, Training, and Evaluating the Model
  - How many neurons, layers, and activation functions did you select for your neural network model, and why?
    - In a first attempt to increase the accuracy of the model the number of neurons was increased from 80 to 100 since 100 was closer to the 3-to-1 ratio of inputs to neurons taking into account the changed number of inputs from the original. In the second attepmt previous changes were kept and the activation function for each of the layers was changed to tanh from relu. In the third attempt previous changes were kept but an aditional layer was added with 10 neurons and the tanh activation. As can bee seen in the images below, none of the three attempts were able to reach a accuracy of at least 75% </br>
    ![This is an image](https://github.com/smwhng/Neural_Network_Charity_Analysis/blob/main/Images/1st.PNG) </br>
    ![This is an image](https://github.com/smwhng/Neural_Network_Charity_Analysis/blob/main/Images/2nd.PNG) </br>
    ![This is an image](https://github.com/smwhng/Neural_Network_Charity_Analysis/blob/main/Images/3rd.PNG) </br>
 
## Summary
