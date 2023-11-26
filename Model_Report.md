## Write a Report on the Neural Network Model:
For this part of the assignment, you’ll write a report on the performance of the deep learning model you created for Alphabet Soup.

The report should contain the following:
  1. Overview of the analysis: Explain the purpose of this analysis.
  2. Results: Using bulleted lists and images to support your answers,   
  address the following questions:

- Data Preprocessing:
  - What variable(s) are the target(s) for your model? :'IS_SUCCESSFUL' column from application_df.

  - What variable(s) are the features for your model? : Is by dropping every other column from application_df --> this was defined by dropping the 'IS_SUCCESSFUL' column from the original dataframe.

  - What variable(s) should be removed from the input data because they are neither targets nor features? : 'EIN' & 'NAME' because they were neither.

- Compiling, Training, and Evaluating the Model
  - How many neurons, layers, and activation functions did you select for your neural network model, and why? : 
  First Attempt - hidden_nodes_layer1 = 8
                  hidden_nodes_layer1 = 5\
  Random numbers were selected to get a starting point for accuracy and ended at 72%.

  Second Attempt - hidden_nodes_layer1 = 10
                   hidden_nodes_layer2 = 10
  Decided to max out the nuerons to see if it would bump up a percent and it did, to 73% accuracy.

  Third Attempt - hidden_nodes_layer1 = 8
                  hidden_nodes_layer1 = 4
                  hidden_nodes_layer1 = 2
  Final attempt was to add an extra layer and increasing the epoch to 125 instead of 100 to see if adding an extra node plus more to run the test model on would help to increase it to 75% accuracy, unfortunatly it did not, ended at  
  
  - Were you able to achieve the target model performance? No
  - What steps did you take in your attempts to increase model performance? Added an extra layer on the third attempt and increased training epochs.

3. Summary: Summarize the overall results of the deep learning model.     
Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation. :

Ended the deep learning model with a 73% accuracy in predicting the classification issue. If the data was possibly cleaned a bit more extensively and closer correlated between the input and output, it would have likely resulted in higher prediction accuracy.