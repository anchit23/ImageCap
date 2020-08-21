# IMAGE CAPTIONING
### 	Given an image, we want to obtain a sentence that describes what the image consists of.

## DATASET
	I have used MSCOCO(Common Objects in COntext) dataset fro training the model.
	COCO is commonly used dataset for image captioning. Every image comes with 5 different captions.
	These captions are used for training the model.

## MODEL
### 	ENCODER
		I have chosen to use the 101 layered Residual Network trained on the ImageNet classification task, already available in PyTorch.
		These models progressively create smaller and smaller representations of the original image, and each subsequent representation is more "learned", with a greater number of channels.

### 	DECODER
		The LSTM component is trained on captions in the dataset.
		Aim is to train the RNN to produce the next word of the sentence based on the previous word. Words are converted to tokens.
		Then the embedding layer transforms each word in a caption into a vector of a desired consistent shape.

![Alt text](https://github.com/anchit23/ImageCap/blob/master/ss.png "My Image as a test Image ")
