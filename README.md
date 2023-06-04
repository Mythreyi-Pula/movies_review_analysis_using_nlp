Sentiment analysis is a powerful tool that allows computers to understand the underlying subjective tone of a piece of writing. This is something that humans have difficulty with, and as you might imagine, it isn’t always so easy for computers, either. But with the right tools and Python, you can use sentiment analysis to better understand the sentiment of a piece of writing.

**Using Natural Language Processing to Preprocess and Clean Text Data**

Any sentiment analysis workflow begins with loading data. But what do you do once the data’s been loaded? You need to process it through a natural language processing pipeline before you can do anything interesting with it.

**The necessary steps include (but aren’t limited to) the following:**

->Tokenizing sentences to break text down into sentences, words, or other units
->Removing stop words like “if,” “but,” “or,” and so on
->Normalizing words by condensing all forms of a word into a single form
->Vectorizing text by turning the text into a numerical representation for consumption by your classifier
->All these steps serve to reduce the noise inherent in any human-readable text and improve the accuracy of your classifier’s results. There are lots of great tools to help with this, such as the Natural Language Toolkit, TextBlob, and spaCy. 

**Vectorizing Text**
Vectorization is a process that transforms a token into a vector, or a numeric array that, in the context of NLP, is unique to and represents various features of a token. Vectors are used under the hood to find word similarities, classify text, and perform other NLP operations.

This particular representation is a dense array, one in which there are defined values for every space in the array. This is in opposition to earlier methods that used sparse arrays, in which most spaces are empty.

Like the other steps, vectorization is taken care of automatically with the nlp() call. Since you already have a list of token objects, you can get the vector representation of one of the tokens

**Using Machine Learning Classifiers to Predict Sentiment**

**How Classification Works:**
Don’t worry—for this section you won’t go deep into linear algebra, vector spaces, or other esoteric concepts that power machine learning in general. Instead, you’ll get a practical introduction to the workflow and constraints common to classification problems.

Once you have your vectorized data, a basic workflow for classification looks like this:

->Split your data into training and evaluation sets.
->Select a model architecture.
->Use training data to train your model.
->Use test data to evaluate the performance of your model.
->Use your trained model on new data to generate predictions, which in this case will be a number between -1.0 and 1.0.
->This list isn’t exhaustive, and there are a number of additional steps and variations that can be done in an attempt to improve accuracy. For example, machine learning practitioners often split their datasets into three sets:

1) Training
2) Validation
3) Test

The training set, as the name implies, is used to train your model. The validation set is used to help tune the hyperparameters of your model, which can lead to better performance.
The test set is a dataset that incorporates a wide variety of data to accurately judge the performance of the model. Test sets are often used to compare multiple models, including the same models at different stages of training.

