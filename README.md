# Predicting-the-critical-temperature-of-superconductors
Predict the critical temperature given some chemical properties of a material?

Introduction

Superconductivity  is  a  phenomenon  of  exactly  zero  electrical  resistance  andexpulsion  of  magnetic  flux  fields  occurring  in  certain  materials,  called  super-conductors, when cooled below a characteristic critical temperature.  Supercon-ductors are widely used in many industry fields, e.g.  the Magnetic ResonanceImaging (MRI) in health care, electricity transportation in energy industry andmagnetic separation, etc.

Predicting the critical temperature (Tc) of a superconductor is still an openproblem in the scientific community. In the past, simple empirical rules based onexperiments have guided researchers in synthesizing superconducting materialsfor many years.  Nowadays, features (or predictors) based on the superconduc-tor’s elemental properties can be generated and used to predictTc.

In this task, we are going to analyze superconductor data from the Super-conducting Material Database maintained by Japan’s National Institute for Ma-terials Science (NIMS). The aim is to build statistical models that can predictTcbased on the material’s chemical properties.Specifically,  you  are  going  to  analyse  a  superconductor  data  set,  which  isbased on real world material science data.  The problem you are going to solve is:  Can you

Predict - the critical temperatureTcgiven some chemical properties of amaterial?
Explain - your  prediction  and  the  associated  findings?   For  example,  describe the key properties associated with the response variable.

The data set was originally from from the Superconducting Material Databasemaintained by Japan’s National Institute for Materials Science(NIMS) and pre-possessed by Kam .  It contains 21,263 material records, each of which have 82columns:  81 columns corresponding to the features extracted and the last 1 col-umn of the observedTcvalues.  Among those 81 columns, the first column is thenumber of elements in the material, the rest 80 columns are features extractedfrom 8 properties (each property has 10 features).  Detailed data preparation process can be found. 

There are two data sets:train.csv can be used to train and validate prediction models and build a description(21,263 material records).  Each record consists of 82 columns,  containing number of elements (column 1), features extracted from 8 properties(columns 2-81) and the critical temperature (column 82). uniquem.csv tells you the chemical formula of each corresponding material.

In order to finish the analyse task, you should split the providedtrain.csvintoyour own training and testing sets before building the models.


Task descriptionIn this assessment, you will focus on the following two tasks.

Prediction task 

For the prediction task, the underlying problem is to estimate the critical temperature given a new conductor’s properties. There are eight properties that canbe used:  Atomic Mass, First Ionization Energy, Atomic Radius, Density, Elec-tron Affinity, Fusion Heat, Thermal Conductivity, Valence.  For each property,ten features are extracted:  Mean, Weighted mean, Geometric mean, Weighted geometric mean, Entropy, Weighted entropy, Range, Weighted range.  Standard deviation, Weighted standard deviation.  The provided data sets are well organ-ised, you do not need to wrangle the data.  But make sure you understand theintuition of these attributes.

To measure the performance of your model(s), you firstly split the original data into training and testing set, fit the model using the training set, do thepredictions on the test set and compute the Mean Squared Error (MSE).

In this task, you are required to develop models that can accurately predicta superconductor’s critical temperature.  To finish the task, you should

1. develop and compare 2 to 3 models;

2.  describe and justify the choice of your models;

3.  analyze and interpret your results.

Description task

The purpose of the description task is identify the key properties for a superconductor.  In other words, which property contributes the most to your model’sperformance?   Descriptions  can  be  based  on  variable  correlation  analysis,  regression equations, linguistic descriptions, or any other form.  The descriptions and the accompanying interpretation must be comprehensible, useful.  To finish this task, you should use proper data analysis techniques (e.g., EDA, statistics)to

1. identify a subset of attributes that have a significant impact on the pre-diction of the critical temperature;

2.  and give statistical reasons of your finding.
