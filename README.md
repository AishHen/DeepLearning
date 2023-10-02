# DeepLearning

**Background**

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

    - EIN and NAME—Identification columns

    - APPLICATION_TYPE—Alphabet Soup application type

    - AFFILIATION—Affiliated sector of industry

    - CLASSIFICATION—Government organization classification

    - USE_CASE—Use case for funding

    - ORGANIZATION—Organization type

    - STATUS—Active status

    - INCOME_AMT—Income classification

    - SPECIAL_CONSIDERATIONS—Special considerations for application

    - ASK_AMT—Funding amount requested

    - IS_SUCCESSFUL—Was the money used effectively


**Process Steps**

Step 1: Preprocess the Data

    A. Read in the charity_data.csv to a Pandas DataFrame

    B. Determined the number of unique values for each column.

    C. For columns that have more than 10 unique values, determined the number of data points for each unique value.

    D. Used the number of data points for each unique value to pick a cutoff point to bin "rare" categorical variables together in a new value Other, and then checked if the binning was successful.

    E. Used pd.get_dummies() to encode categorical variables.   

    F. Split the preprocessed data into a features array, X, and a target array, y. Used these arrays and the train_test_split function to split the data into training and testing datasets.

    G. Scale the training and testing features datasets by creating a StandardScaler instance, fitting it to the training data, then using the transform function.

Step 2: Compile, Train, and Evaluate the Model

    A. Created a neural network model by assigning the number of input features and nodes for each layer using TensorFlow and Keras

    B. Created the first and second hidden layers and chose the ReLU activation function.

    C. Created an output layer using the Sigmoid activation function.

    D. Compiled and trained the model

    E. Created a callback that saves the model's weights every five epochs

    F. Evaluated the model using the test data to determine the loss and accuracy

Step 3: Optimize the Model
    Used the following methods to optimize the model:
        Dropped non-essential columns.
        Added more neurons to the hidden layers.
        Added hidden layers.
        Added epochs to the training regimen.


**Resources Used**
1. TA Office Hours - Nathan Darter
2. Class Material - Unit 21 Exercises

**References**
IRS. Tax Exempt Organization Search Bulk Data Downloads. https://www.irs.gov/ Links to an external site.

