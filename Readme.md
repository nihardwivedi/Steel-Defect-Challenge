# Steel-Defect-Challenge
> Github repo for the Kaggle Steel Challenge.  
>
> - Team members are **Nihar Dwivedi** and **Toluwaleke Olutayo**.<br/>

#### Product Definition<br/>

#### Product Mission: <br/>
For Steel manufacturers and construction companies, who need to efficiently identify defects in steel, Steel Defect Detector is a machine learning module that classifies defects in steel sheets.<br/>

#### Target Users <br/>
Manufacturing companies/suppliers
Construction managers<br/>

#### User Stories <br/>
As a construction manager, I want to be able to quickly identify defects in steel so that I can save money and time by quickly alerting the suppliers and getting a replacement.

As a manufacturer, I want to be able to prevent potential disasters due to sub-quality steel. 

As a supplier, I want to be able to supply my customers with quality steel so as to become/remain profitable.

#### MVP-<br/>
A working classifier.

#### User Interface(Optional)<br/>
Product Survey
Existing Similar Products
Accuracy is a very important measure measurement for the model. SaurabhG(2018) mentioned that the gradient boosting classifier had the highest testing accuracy, after comparing five different algorithms. It also introduce the NEU data base to us. The data set  has divided the image into six data set.
Hu, H et al(2014) claims that the support vector machine performed better than the neural networks in the average class accuracy, especially for the case with limited classes. 
To learn more existed Kaggle Competition, we find that the lung cancer detection has similar point with our project, and we will use it in sprint3. As for sprint1, we based on literature research and the adjustment of high rank solution, which will be discussed in the code mamagent part.<br/>

#### Patent Analysis<br/>

#### References<br/>
Krizhevsky, A., sUTSKEVER, B., & Hinton, G. E. (n.d.). Image classification with deep convolutional neural networks.
Hu, H., Li, Y., Liu, M., & Liang, W. (2014). Classification of defects in steel strip surface based on multiclass support vector machine. Multimedia Tools and Applications, 69(1), 199-216.<br/>
Sarma, A. S. S., Janani, R., & Sarma, A. S. V. (2013, September). Detecting the surface defects on hot rolled steel sheets using texture analysis. In 2013 International Conference on Advanced Electronic Systems (ICAES) (pp. 157-159). IEEE.<br/>

#### System Design<br/>

Data -> Exploration -> Classification -> Verification

##### Major Components<br/>

There are 2 major components of the system-<br/>

###### The Data <br/>
that will be needed for the development, processing, and verification of the model. 
 This is provided in the form of a dataset of 50k images by the kaggle competition host.
The dataset consists of a training set that can be downloaded for model training, as well as a test set that can't be downloaded, but will be used in the online verification process to calculate the accuracy of the model.
The dataset contains unlabelled images and a few labeled images. This means both unsupervised and supervised learning can be applied here. A comparison of the accuracy of the two will lead to final method selection.<br/>
The Model itself. We'll be developing a model that uses a machine-learning algorithm to analyze images of a steel sheet surface that detects and classifies the defects into categories.<br/>
##### The model <br/>
will be a Jupyter notebook, explaining the steps it takes, and code it uses for the steps like image segmentation, feature extraction, defect detection and classification.
The training and test phases of the model might be done offline prior to submission, to make use of GPUs for maximum training speed.
The submission of the model is however done online, where it is run against the test dataset for accuracy calculation, and the top scorers are assigned a rank on the leaderboard.<br/>

##### Technology Selection(Reason & Comparisons, Optional for a while)
Machine Learning has multiple frameworks that we can use. We had to choose between PyTorch, Tensorflow and Kaffe. We went with pytorch because of its widespread adoption, huge developer community, and support.<br/>

##### Test or Verification Program
The Model will be tested against a hidden database and accuracy calculated by comparison with the ground truth. The ranking of the submission will be the validation.

##### Sprint 1
##### Link to presentation - https://docs.google.com/presentation/d/19450wHM0ajLizVtfXvIG-2JWzgNhxDii_kCdJUwvPZU/edit?usp=sharing

##### Sprint 2
##### Link to presentation - https://docs.google.com/presentation/d/1ImDJBQAi0kkcxEllg10kABklKd0c9ALbCp6_KfMNbgQ/edit?usp=sharing
