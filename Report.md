## Overview
* The purpose of this project was to predict whether applicants will be successful if they are fuded by Alphabet soup. This machine learning would be a tool used by Alphabet soup to pick the best candidates for funding.
## Results

# Data Preprocessing

What Variable was the target for the model? 
* Is_Successful was the target for the model

What Variables were the features for the model?
* Application_Type
* Affiliation
* Classification
* Use_Case
* Organization
* Status
* Income_AMT
* Special_Considerations
* Ask_AMT

What Variables should be removed from the input data becuase they are neither targets nor features?
* EIN
* NAME


# Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural netowrk model, and why? 
In the first run, I used two hidden layers with 80/30 neurons respecitvely with relu activation and sigmoid output activation. I went with relu/sigmoid as the data appeared to be non-linear. I went with 80/30 neurons as a solid starting level as this is similar to what we did on previous challenges. 

* Were you able to achieve the target model performance?
The first model achieved an accuracy of .7255 which fell short of the .7500 target goal. 

* What steps did you take in your attempts to increase model performance?
With the first model failing, I made various changes to the next models listed below:

Model 2: 
- Changes: 
* Added a 3rd hidden layer with 10 neurons, and relu activation. All other variables remained the same. 
- Results: 
* Accuracy decreased slightly to .7254

Model 3: 
- Changes: 
* Kept 3rd hidden layer, changed all neurons to 100
- Results: 
* Accuracy increased slightly to .7261

Model 4: 
- Changes: 
* Kept changes from Model 3, changed cutoff value for the feature variables 
- Results: 
* Accuracy decreased slightly to .7238


## Summary
Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
* To summarize, all 4 models failed to hit the target goal of .7500 accuracy with the closest being Model 3 at .7261. I believe I should have made some harsher changes to the later models such as changing activation methods and playing more with the hidden layers. My recommendation would be to change activation methods and maybe try some different learning models to see the impact