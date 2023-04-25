# TheHeartSoundHerd

Attached in this submission are: presentation powerpoint, README.md, HeartSoundClassifier_CNN_1D.ipynb, Cardiac_Segmentation_v2.ipynb

### HeartSoundClassifier_CNN_1D.ipynb
HeartSoundClassifier_CNN_1D.ipynb contains the code that trained and saved the models. In this file, for both the original model and transfer learning: the data was loaded and pre-processed (sample rate change, removing short files, cutting long files), datasets with data augmentation were defined, the model architecture was defined, training loop was written out, and evaluation was performed.

### APPENDIX: Cardiac_Segmentation_v2.ipynb
Cardiac_Segmentation_v2.ipynb contains some exploratory analysis. There was experimentation between two data noise reduction methods (low-pass butterworth filter, performed by apply_lowpass_filter() and a noise reduction by spectral subtraction method, performed by noise_reduction()). Some samples from physionet, dataset A, and dataset B were displayed (unprocessed, and processed by each of the two methods) for visual analysis. Recordings were displayed so that we could learn the data and understand the categories while visualizing the data.
Lastly, there was experimentation with phonocardiogram segmentation. We were planning to run segmented heart sounds through the model, but we found that running a 1D convolutional model was sufficient. However, this could be a direction of future study of how to improve the model.
