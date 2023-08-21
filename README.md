# deep-learning-challenge
 

### Overview of the analysis
The purpose of this analysis was to build, train, and test a neural network that accurately could predict the result (successful vs non successful) of a nonprofit organization. This was done through three main steps: processing the data, compiling and training a model, and finally optimizing the model. 

### Data Preprocessing
#### What variable(s) are the target(s) for your model?
   The target variable was the binary "success" variable

#### What variable(s) are the features for your model?
   APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT,                SPECIAL_CONSIDERATIONS, and ASK_AMT 

#### What variable(s) should be removed from the input data because they are neither targets nor features?
   I removed the name and the EIN as they were not relevant to the analysis. 


### Compiling, Training, and Evaluating the Model

#### How many neurons, layers, and activation functions did you select for your neural network model, and why?

Originally, I only added an initial layer, one hidden layer, and an output layer. Each of these layers had only one neuron and used the "sigmoid" function, as this was a classification problem. Because of the immense number of columns that I was left with after adapting the data set to have dummy variables, I wanted to keep my model simple as a baseline to jump off of. 

#### Were you able to achieve the target model performance?

My goal was to achieve an accuracy of at least 75%, and in my first model attempt I did not achieve this. I did get pretty close, with an accuracy of 73%.

#### What steps did you take in your attempts to increase model performance?

I tried a few different steps to optimize this model, including adding more neurons, adding more hidden layers, and upping the number of epochs used to fit the model. Unfortunately, none of these steps were enough to significantly improve my accuracy. 

### Conclusion
Through the process of this project, while I was unable to achieve target accuracy, I do have ideas for other ways to optimize this model. I think that using PCA to reduce the number of input variables would be a good way to possibly raise accuracy. Or, one could change the cutoff bins for a few of the variables. Additionally, if more time and computing power was available, one could again increase the number of neurons and hidden layers. 

If I were to use another method to solve this problem, I would probably use a random forest, as this is a classification problem with a lot of input variables, and I think that using a random forest could be successful. 
