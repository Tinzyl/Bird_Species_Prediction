# Bird_Species_Prediction
### In this project, I used a Convolutional Neural Network to predict the species of a Bird. The Sequential Model that is provided by the Keras library is the one which was used to build the Convolutional Neural Network. The number of epochs that were used to train the data were 50 and the batch size was 128. The data that I used was from [Kaggle](https://www.kaggle.com/gpiosenka/100-bird-species?select=test). Due to computational power, I only picked 5 species, hence I had 5 classes. These were:

1. African Crown Crane
2. African FireFinch
3. American Coot
4. Baltimore Oriole
5. Varied Thrush

### Steps which were taken to build the project were as follows:
- Performed Data Visualization on the Bird Images
- Made sure that all the images were the same dimensions so that the fitting of the model and the prediction could be efficient
- Converted the images into a numpy array, and then I normalized the images
- Checked if there was any class imbalance or not
- Split the data into 80% training data and 20% test data
- Performed one-hot encoding inorder to turn the bird categories into binary categories that can be fit into the model
- Created the model, added the layers, compiled it and fit the data
- Plotted the accuracy and loss graph for each epoch
- Preprocessed the test data, and made predictions on it
- Visualized the predicted labels against the original labels.

## Results
I applied early stopping, and the model stopped improving it's accuracy after 30 epochs, hence that is when it stopped training. 
The graph which shows how the accuracy of the training and validation data changed with the number of epochs is shown below:
![Unknown](https://user-images.githubusercontent.com/18570056/147376022-231689c9-989d-419b-a5b1-9854db0f8252.png)

The graph which shows how the loss of the training and validation data changed with the number of epochs is also shown below:

![Unknown-2](https://user-images.githubusercontent.com/18570056/147376036-c3a639bf-2375-423d-b872-44b930b21bd2.png)

When tested on the Test dataset, the accuracy was: **77.12%**.
