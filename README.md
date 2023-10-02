# Introduction

This is an implementation of submitted paper:  
Scheduled post  
Masayuki Kogoshi, Daiki Nishio, Nobutaka Kitahata, Hayato Ohwada, Kazuyuki Kuchitsu, Hideyuki Mizuno1 and Takamitsu Kurusu.  
Novel in silico screening system for plant defense activators using deep learning-based prediction of reactive oxygen species accumulation.  

drug_ros_RF.ipynb  
Random forest is used to learn the ROS values generated by spraying compounds on plants and the chemical features of each compound to infer the amount of ROS generated by the compound.

drug_ros_smote  
Infer the amount of ROS produced by a compound by using a DNN to learn the ROS values generated by spraying compounds on plants and the chemical features of each compound.

GTM_drug_chemical_space  
Display chemical features of each compound in two dimensions using GTM (Generative Topographic Mapping) method


# Features

In this method, ROS modulators, which are potential plant defense activators, were accurately predicted with a high level of precision, exceeding 90% .  
The reason for the high accuracy is thought to be that the candidate compounds are amplified by the SMOTE method before training and verification, it is likely that chemical features similar to the candidates will be included in the training data. The high level of  accuracy can be attributed to the amplification of candidate compounds through the SMOTE method prior to the training and validation processes, thereby increasing the likelihood of incorporating chemical characteristics similar to the candidate into the training dataset. 

# Results
https://github.com/ma1206ko/in_silico_screening/blob/main/image/Fig3_DNN.tif
