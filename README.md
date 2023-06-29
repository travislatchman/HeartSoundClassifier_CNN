# The Heart Sound Herd: Classifying Abnormalities in Phonocardiograms

Attached in this submission are: presentation powerpoint, README.md, HeartSoundClassifier_CNN_1D.ipynb, Cardiac_Segmentation_v2.ipynb

### HeartSoundClassifier_CNN_1D.ipynb
HeartSoundClassifier_CNN_1D.ipynb contains the code that trained and saved the models. In this file, for both the original model and transfer learning: the data was loaded and pre-processed (sample rate change, removing short files, cutting long files), datasets with data augmentation were defined, the model architecture was defined, training loop was written out, and evaluation was performed.

### HeartSoundClassifier_CNN_1D_additional.ipynb
Due to random initializations, HeartSoundClassifier_CNN_1D.ipynb does not have all of the output that we discuss in the presentation; these are found in HeartSoundClassifier_CNN_1D_additional.ipynb.

### APPENDIX: Cardiac_Segmentation_v2.ipynb
Cardiac_Segmentation_v2.ipynb contains some exploratory analysis. There was experimentation between two data noise reduction methods (low-pass butterworth filter, performed by apply_lowpass_filter() and a noise reduction by spectral subtraction method, performed by noise_reduction()). Some samples from physionet, dataset A, and dataset B were displayed (unprocessed, and processed by each of the two methods) for visual analysis. Recordings were displayed so that we could learn the data and understand the categories while visualizing the data.
Lastly, there was experimentation with phonocardiogram segmentation. We were planning to run segmented heart sounds through the model, but we found that running a 1D convolutional model was sufficient. However, this could be a direction of future study of how to improve the model.  

![image](https://github.com/travislatchman/HeartSoundClassifier_CNN/assets/32372013/4cc059b4-74ea-4431-aaa4-543080b8ac95)  
![image](https://github.com/travislatchman/HeartSoundClassifier_CNN/assets/32372013/579ca878-0037-4aba-87ba-11c5aede9db2)  
![image](https://github.com/travislatchman/HeartSoundClassifier_CNN/assets/32372013/b0eb1efb-449f-411e-a226-2eb1497829fd)  
![image](https://github.com/travislatchman/HeartSoundClassifier_CNN/assets/32372013/39986737-8bb7-4c01-a1ba-8df614b9df9e)  
![image](https://github.com/travislatchman/HeartSoundClassifier_CNN/assets/32372013/074d2fe0-61b5-4c65-8fa1-63cdbc668c58)  
![image](https://github.com/travislatchman/HeartSoundClassifier_CNN/assets/32372013/0ff171ac-cb79-4762-b81d-827adf6eb5ff)  
![image](https://github.com/travislatchman/HeartSoundClassifier_CNN/assets/32372013/101ffcdf-c0ef-4667-a49a-58b8d81389c9)  
![image](https://github.com/travislatchman/HeartSoundClassifier_CNN/assets/32372013/cff68941-b817-4df5-a48a-f3bdc3df5619)  



