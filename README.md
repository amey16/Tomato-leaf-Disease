# Tomato-leaf-Disease
kaggle project
# Dataset 
The dataset was picked from kaggle - [link](https://www.kaggle.com/noulam/tomato) <br/>
The dataset has two directories with train data and validation data as the test data <br/>
There are 10 different types of diseasis present in the data

# Algorithm used
Transfer Learning was used to do this particular project <br/>
InceptionV3 came out to be the best model.Restnet and VGG16 din't perform well <br/>
Architecture of the model is somewhat like - <br/>
![image](https://user-images.githubusercontent.com/51751926/124195601-6499c900-dae8-11eb-84f9-4ecbd08c63e1.png)

<br/>
As there is only one input and output in this particular model we don't use that  <br/>
Data being catagorical instead of binary input and output layers are self made and wrapped with model using sequential 

# Results and Improvements
- I could not properly train the model due to no gpu in my laptop although achieved 84% accuracy 
- To train the model change the steps_per_epoch to len(trainset) and you will get better accuracy
- Preferable to do this particular project in google colab
- Flask app can be made which takes an image of infected tomato leaf and predict the type of disease
