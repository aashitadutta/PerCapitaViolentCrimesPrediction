# Per Capita Violent Crimes Prediction
Per capita violent crimes prediction on the  <a href="http://archive.ics.uci.edu/ml/datasets/communities+and+crime">Communities and Crime Dataset</a> from UCI Machine Learning.
* Genetic Algorithm is used for feature selection. 
* Data is then descritized using pandas cut function into bins.
* Decision trees are used for the rules generation.
* Rules generated are used in the Fuzzy Inference System developed in matlab.
* Accuracy is tested.
## Team Members : 
* [Abhilash Gahankari](https://github.com/abhilashgahankari) [2020H1030113H]
* [Aashita Dutta](https://github.com/aashitadutta) [2020H1030130H]
* [Satish Phale](https://github.com/satishphale) [2020H1030155H]
* [Harsha Varun](https://github.com/varunmarisetty) [2020PHXP0437H]

# Feature Selection Using GA
An example implementation of a simple Genetic Algorithm applied to feature selection. It will be using the Communities and Crime Dataset from UCI Machine Learning, which has 128 attributes, aimining to use these attributes in order to predict the label (Per Capita Violent Crimes). We will use the Genetic Algorithm to select which of those 128 features are most relevant to this prediction.

# Discretization
After features selected by genetic algorithm, continuous values are dicretized into range values using pandas cut function into bins and encoded into class variables.
# Rules Generation
Generating Rules from Discretized+Encoded data optimized using Genetic Feature Selections. sklearn.tree.DecisionTreeClassifier¶ is used to generate rules in text format with distinct classes based on probability, number of samples and gini index to measure how impure the partitions are.
![image](https://user-images.githubusercontent.com/6908904/121800938-3d22af80-cc52-11eb-8cdb-3d510073a90e.png)

# Fuzzy Inference System
Rules along with data are fed into Fuzzy Inference System in MATLAB, where trapezoidal function is used as membership function for fuzzification and trules inference system and centrold method is used for defuzzification. Accuracy measures gives best value for medium class.
