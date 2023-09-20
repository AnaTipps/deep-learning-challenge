# Deep Learning Challenge 

![Alt text](image.png)

# Background
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization

# Analysis Preprocess

## Step 1: Preprocess the Data
Using 'Pandas' and 'scikit-learn’s' 'StandardScaler()', the dataset were preprocessed. This step its a prep for Step 2, where I compiled, trained, and evaluated the neural network model.

I started by uploading the starter file to Google Colab, then using the information provided in the Challenge files, follow the instructions to complete the preprocessing steps.

1. The charity_data.csv was read to a Pandas DataFrame, and the following was be sure identify in dataset:
    + What variable(s) are the target(s) for your model?
    + What variable(s) are the feature(s) for your model?

2. Some unecesary columns were droped ('EIN' and 'NAME' columns).

3. The number of unique values for each column were determined .

4. For columns that had more than 10 unique values, the number of data points for each unique value were determined.

5. The number of data points for each unique value were picked and used as cutoff point to bin "rare" categorical variables together in a new value, Other, and then check if the binning was successful.

6. The 'pd.get_dummies()' function was used to encode categorical variables.

7. The preprocessed data was splited into a features array, 'x', and a target array, 'y'. Use these arrays and the 'train_test_split' function to split the data into training and testing datasets.

8. By creating a 'StandardScaler' instance the datasets Scale the training and testing features datasets , fitting it to the training data, then using the 'transform' function.

## Step 2: Compile, Train, and Evaluate the Model

Using TensorFlow, a neural network was designed, or deep learning model, to create a binary classification model that can predict if an Alphabet Soup-funded organization will be successful based on the features in the dataset. It needs to be consider how many inputs there are before determining the number of neurons and layers in the model. Once that step is completed, you’ll compile, train, and evaluate your binary classification model to calculate the model’s loss and accuracy following the steps below.

1. Continue using the file in Google Colab in which you performed the preprocessing steps from Step 1.

2. Create a neural network model by assigning the number of input features and nodes for each layer using TensorFlow and Keras.

3. Create the first hidden layer and choose an appropriate activation function.

4. If necessary, add a second hidden layer with an appropriate activation function.

5. Create an output layer with an appropriate activation function.

6. Check the structure of the model.

7. Compile and train the model.

8. Create a callback that saves the model's weights every five epochs.

9. Evaluate the model using the test data to determine the loss and accuracy.

10. Save and export your results to an HDF5 file. Name the file 'AlphabetSoupCharity.h5'.

## Step 3: Optimize the Model

Using TensorFlow, optimize your model to achieve a target predictive accuracy higher than 75%.

The following methods can be used to optimize the model:

Adjust the input data to ensure that no variables or outliers are causing confusion in the model, such as:
Dropping more or fewer columns.
Creating more bins for rare occurrences in columns.
Increasing or decreasing the number of values for each bin.
Add more neurons to a hidden layer.
Add more hidden layers.
Use different activation functions for the hidden layers.
Add or reduce the number of epochs to the training regimen.
Note: If you make at least three attempts at optimizing your model, you will not lose points if your model does not achieve target performance.

1. A new Google Colab file will need to be createad and name it 'AlphabetSoupCharity_Optimization.ipynb'.

2. Import your dependencies and read in the 'charity_data.csv' to a Pandas DataFrame.

3. Preprocess the dataset as you did in Step 1. Be sure to adjust for any modifications that came out of optimizing the model.

4. Design a neural network model, and be sure to adjust for modifications that will optimize the model to achieve higher than 75% accuracy.

5. Save and export your results to an HDF5 file. Name the file AlphabetSoupCharity_Optimization.h5.

## Step 4: Write a Report on the Neural Network Model
A report is attached on the performance of the deep learning model created for Alphabet Soup.

The report contains the following:

1. ** **Overview** **  of the analysis: Explain the purpose of this analysis.

2. ** **Results** ** : Using bulleted lists and images to support your answers.

3. ** **Summary** **: Summarize the overall results of the deep learning model. 


