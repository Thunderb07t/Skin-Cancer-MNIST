# Skin-Cancer-MNIST
To analyse, process and classify images in Kaggle Skin Cancer MNIST dataset using Transfer Learning in Pytorch.

In the Skin_Cancer_MNIST jupyter notebook, the kaggle dataset Skin Cancer MNIST : HAM10000 has been used.
Link to the dataset : https://www.kaggle.com/kmader/skin-cancer-mnist-ham10000
Skin cancer MNIST dataset contains 10000 images of skin lesions each of which can be classified into 7 classes.

Note : For the purpose of this notebook , extract the dataset and then extract the contained images zip files to 'Images' folder.

Here the transfer learning is being used, for this we have used the Densenet-121 model which is available in torchvison.models.
 Densenet uses interconnected convolution layers as the feature extractor. And hass a linear classifier to which features are fed.
For more details refer to : 
	https://github.com/pytorch/vision/blob/master/torchvision/models/densenet.py
  https://pytorch.org/docs/stable/_modules/torchvision/models/densenet.html
	

The model is trained using The Negative- Log-Likelihood loss and ADAM optimizer with learning rate = 0.001.
Also the dataset has been divided into batches of 32.

The model is trained and validation accuracy of 80.7% is obtained after running inly 1 epoch and accracy of >90% can be achieved by running 10-15 epochs.
