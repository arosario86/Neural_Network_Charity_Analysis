# Neural_Network_Charity_Analysis
## Overview
I have been tasked to work with Beks on creating a binary classifier that will helo her predict whether the applicants would be successful if they were funded by Alphabet Soup. The CSV she provided has over 34,000 organizations and we had to work on preparing the data before running any machine learning models.
## Results
I did the following before running the models:
    * Dropped non-beneficial columns such as 'EIN' and "NAME'
    * Determined unique values for each column
    * Viewed application type counts
    * Visualize the counts
    
    ![Value Counts](https://user-images.githubusercontent.com/104965708/200996209-5f38c19f-899a-4657-a37b-13beae11ed20.png)
    
    * Determined which values to replace in the application counts
    * Viewed classification counts
    
    ![Classification Counts](https://user-images.githubusercontent.com/104965708/200996349-e7966618-32e8-4ebd-ad7f-8ca5044a0133.png)
    
    * Determine which values to replace in the classification counts
    * Generated categorical lists
    * Created a One Hot Encoder
    * Merge one hot encoder and drop originals
    * Split the processed data into features and arrays 
    * Create a standard scaler for the data

## Summary
Once the data was prepared and ready to train, I did the following to test the models:
* I compiled, trained, and evaluated the model
    * The first hidden layer had 80 units, the second hidden layer had 20 units, and the output layer had 1 unit. This resulted in the total parameters being 5,241.

![model](https://user-images.githubusercontent.com/104965708/200995721-51724906-dde1-4916-90e9-37aaf600f2cf.png)

* This model had an accuracy of 74%

![Accuracy](https://user-images.githubusercontent.com/104965708/200996907-136a5f49-f9b5-4ee7-910b-74e96e0a0ffe.png)

![Loss and Accuracy](https://user-images.githubusercontent.com/104965708/200996927-6ba8939b-92db-449e-95f8-b458190a3b7e.png)

Once the first model was completed, I used the original data to create an optimized version and tested additional hidden layers in an attempt to get a 75% or higher accuracy.
* The first hidden layer had 180 units, the second hidden layer had 80 units, the third hidden layer had 40 units, and the output layer had 1 unit. This resulted in the total parameters being 25,861.

![Optimized Model 1](https://user-images.githubusercontent.com/104965708/200997318-18ef637b-ca24-4838-86bb-7f3094dd8352.png)

![Optimized Model 2](https://user-images.githubusercontent.com/104965708/200997270-02dc9dfc-7426-4316-8108-b3c0fc3041f1.png)

* This model had an accuracy of 74% as well.

![Optimized Loss and Accuracy](https://user-images.githubusercontent.com/104965708/200997487-df37f750-082e-444e-b343-d9c13a2e6cf3.png)

Recommendations:
The data, the model, and its accuracy score are not high enough to feel confident. 74% seemed to be the highest rate of accuracy I could achieve when playing with the units and models. I would recommend to use Random Forest Classifier to try and improve the accuracy of the prediction.
