# deep-learning-challenge
# Report on the Neural Network Model
The purpose of this analysis: I did this anlaysis aiming yo help the Alphabet foundation to select the best applicant for founding, i design an artificial neural network with different layer, neurons, changing the input a little bit, aiming to get better accuracy,
Results: Using bulleted lists and images to support your answers, address the following questions:

Data Preprocessing

What variable(s) are the target(s) for your model?
The target variable is the 'IS_SUCCESSFUL' column from application_df

y = application_dummies['IS_SUCCESSFUL']

What variable(s) are the features for your model?
The feature variables are every other column from application_df --> this was defined by dropping the 'IS_SUCCESSFUL' column from the original dataframe

X = application_dummies.drop(['IS_SUCCESSFUL'], axis=1)


What variable(s) should be removed from the input data because they are neither targets nor features?
Both 'EIN' and 'NAME' columns were dropped/removed, because they were neither targets nor features for the dataset.

Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
In the first attempt, I used 10 hidden_nodes_layer1 and 5 hidden_nodes_layer2  and one node output layer-- these were just random guesses from which to iterate upon in the second try


Were you able to achieve the target model performance?
After 100 epochs the proposed model was only able to acheive only accuracy of: 0.7311

What steps did you take in your attempts to increase model performance?
I experimented with increasing nodes and neurons, with changing other parameters to get a better accuracy but despite doing this both models came below the 75% threshold. finally i did not drop the names columns trying to get better accuracy.

Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

Overall,  to improve the deep learning model's performance, I would consider adding more data, ensuring proper data cleaning, exploring alternative algorithms, identifying feature importance, addressing bias and outliers, and applying data binning techniques. Each step aims to enhance the model's ability to capture relevant patterns and reduce noise, ultimately improving accuracy in the classification problem. It is important to iterate and experiment with these steps, evaluating the impact on model performance and fine-tuning as necessary.
