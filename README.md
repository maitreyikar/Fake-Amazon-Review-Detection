# Fake-Amazon-Review-Detection

1. Our proposed model uses a publicy available amazon review dataset from kaggle (https://www.kaggle.com/datasets/lievgarcia/amazon-reviews). The file can be found at "datasets/amazon_reviews.txt"

2. In order to capture the relationship between spurious reviews and emotion representation, 30 emotion features were extracted from the "datasets/amazon_reviews.txt" using 9 emotion lexicons. The resultant features were added to the dataset and saved as "datasets/amazon_reviews_features.txt"

3. The code used to extract the aforementioned emotion features can be found in "Emotion_Feature_Generation.ipynb". Recomputing these features requires Java 1.6+. It also requires downloading of all the lexicons mentioned in "Emotion_Feature_Generation.ipynb". Our advice would be to NOT execute "Emotion_Feature_Generation.ipynb" as it consumes significant disk space and time.

4. The code for the rest of the project (including preprocessing, remaining feature extraction, model training, validation) can be found in "Fake_Review_Detection.ipynb" (this uses "datasets/amazon_reviews_features.txt"). It has the following dependencies:
	a. nltk
	b. pandas
	c. re
	d. sklearn
	e. matplotlib
	f. gensim
	g. tensorflow




