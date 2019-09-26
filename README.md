# Machine-Learning-Project
This project is to classify a dataset of grey-scale images to different labels with supervised classifiers. We first pre-process the data with Normalisation and Principal Component Analysis(PCA), then classify our data with K-Nearest-Neighbors (KNN) and Logistic Regression using One-Versus-One (OVO) and One-Versus-All (OVA) methods.

The dataset consists of 30,000 grey-scale images each with the shape of 28x28. The images are classified into 10 labels.

The .ipynb file includes all the code with three methods, OVO of logistic regression, OVA of logistic regression, and knn method.

Run each code cell from the first the last one, which the main function is included. 
The last cell draws the confusion matrix of the results.
  
For the main function, mnist_predicate
(train_set_x, train_set_y, test_set_x, test_set_y, model_name, optimisation_name), 
train_set_x,train_set_y,test_set_x,test_set_y are the preprocessed train x ,y and test x,y
model_name is the model you choose, and optimisation_name is the optimisation method you write in.
you can choose one of the following model :"OVO","OVA"and "KNN" ,
you can choose the following optimisation method :"Momentum","TNC","gDescent".

hence the composisitions could be :
mnist_predicate(train_set_x,train_set_y,test_set_x,test_set_y,"OVO","TNC ") 
mnist_predicate(train_set_x,train_set_y,test_set_x,test_set_y,"OVO","Momentum") 
mnist_predicate(train_set_x,train_set_y,test_set_x,test_set_y,"OVO","gDescent") 
mnist_predicate(train_set_x,train_set_y,test_set_x,test_set_y,"OVA"," ") 
mnist_predicate(train_set_x,train_set_y,test_set_x,test_set_y,"KNN"," ") 

The predicated result of the model is returned from the main function.
The total time used for training and the accuracy is also shown.
