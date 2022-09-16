# Movie-Reviews-Multi-Class-Text-Classification

I finally have a working Multi Class Text Classification model. Used [BERT](https://en.wikipedia.org/wiki/BERT_(language_model)) model from the [transformers](https://pypi.org/project/transformers/) python module which provides thousands of pretrained models to use for NLP and Computer Vision tasks.
As transformers package is not pre installed in Colab, you have to manually install it, the data is in the `train.tsv` file and it contains over 156,000 moview reviews, each marked with its corresponding sentiment in `sentiments` column. There are 5 total sentiments which are

0 - negative

1 - somewhat negative

2 - neutral

3 - somewhat positive

4 - positive

Both Tokenizer and the model are loaded with pre trained weights. I did not validate the model during training but it did pretty well even after training for one epoch. After preprocessing the dataset is in `tf.dataset` format with over 9700 data units. Estimated time for for training on just 1000 units for every epoch is over 13 minutes.
