# Image-Captioning

so this is a group project and we tried to make a model which will be able to caption unseen images.

we used flickr8k as our dataset, since the dataset is small the performance is not great but if flickr30k is used instead of flickr8k then we can see significant performance improvemet.

we used MobileNet as our base model but we also tried VGG16 and few others and got similar performance in all of them. First we pre-processed and cleaned the images then we feed it to our base model i.e, MobileNet which generated the feature vector. We feed the feature vector to RNN which predicted the captions. but before feeding it to RNN we need to create a dictionary out of the captions in our dataset and converted each unique word into a number so that our model can understand the caption.

we used bleu score as our scoring parameter and we achieved a bleu score of 0.65

all of the code is in ipynb file
