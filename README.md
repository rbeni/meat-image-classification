# meat-image-classification

Example code for a CNN image classifier or meat images

This is a simple CNN base classifier, built upon a pre-trained EfficientNetB0.

The dataset used for this model is not included here, but can be obtained from roboflow via the following link:
> https://universe.roboflow.com/i-wayan-adi-saputra-79v4k/beef-quality-detection

## Training

This model as tested with EfficientNet bases from B0 to B4 and from no hidden layer in the classifier to the current 3. Less layers resulted in poor training quality, meaning that the network needed to be more complex to represent the distribution of data seen in the dataset. 

Other types of CNN bases layers were not attempted.

## Usage

To run this notebook, download the notebook file on this repository and the dataset from roboflow. I placed the contents of the zipfile inside a folder named /data, but you can choose other style of organization. Just be aware that you will have to change the paths indicating where the ImageDataGenerators will pull the files from.

Then, install the packages as they are listed on the requirements.txt file

## Improvements

This is a list of the nexts steps for this project:

* ~~Test with different base layers~~
* ~~Include callbacks (best model, early stopping) during the training~~
* ~~Save the model to file~~ Model saved, but not included due to size
* Transfer to tensorflow lite and check differences in inference time
* Check a heatmap to discover which features are more important to each class


