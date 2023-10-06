# Introduction

This is an implementation of submitted paper:  
Scheduled post  
Masayuki Kogoshi, Daiki Nishio, Nobutaka Kitahata, Hayato Ohwada, Kazuyuki Kuchitsu, Hideyuki Mizuno1 and Takamitsu Kurusu.  
Novel in silico screening system for plant defense activators using deep learning-based prediction of reactive oxygen species accumulation.  

### research summary
Plant defense activators offer advantages over pesticides by avoiding the emergence of drug-resistant pathogens. However, only a limited number of compounds have been reported. 
Reactive oxygen species (ROS) act as not only antimicrobial agents but also signaling molecules that trigger immune responses. They also affect various cellular processes, highlighting the potential ROS modulators as plant defense activators.  
We established a new in silico screening system for plant defense activators using deep learning-based ROS accumulation prediction combined with compound chemical properties as explanatory variables.  
As a result of evaluating the accuracy of compounds predicted using molecular biological methods such as pathogenic signal-induced enzyme ROS induction and programmed cell death as an immune response, Our deep learning-based screening systems can rapidly and effectively identify potential immune signal-inducible ROS modulators with distinct chemical characteristics compared with the actual ROS measurement system in plant cells.  


# Requirement
The libraries used in this research are as follows.   
* python 3.7.9
* dcekit 2.4.4
* imbalanced-learn 0.7.0
* keras 2.2.4
* scikit-learn 0.23.2
* tensorflow 1.15.0

# How to run
All programs are ready to run on jupyter notebook!  
The data file required by all program exists in "data" directory.  
If change the location of data file, you must properly set path variables to new path.  

### drug_ros_RF  
Data are amplified by the SMOTE method before training. Then learning and estimation of ROS values by Random Forest.  
47 compound features are used as input data.  

### drug_ros_smote  
Data are amplified by the SMOTE method before training. Then learning and estimation of ROS values by Random Forest.  
Input data is the same as drug_ros_RF.  

### GTM_drug_chemical_space  
Display chemical features of each compound in two dimensions using GTM (Generative Topographic Mapping) method.

# Results
The execution results for the DNN test data are as follows.  
<img src="https://github.com/ma1206ko/in_silico_screening/blob/main/img/DNN.jpg" width="800" />


The results of displaying the chemical space of 9991 test data in GTM are as follows.  
<img src="https://github.com/ma1206ko/in_silico_screening/blob/main/img/GTM_chemical_space.jpg" width="800" />
