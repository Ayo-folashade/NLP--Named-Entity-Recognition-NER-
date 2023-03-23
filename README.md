# Named Entity Recognition with LSTM Neural Network

This code provides an implementation of a Long Short-Term Memory (LSTM) neural network for Named Entity Recognition (NER). The code uses a ner dataset, which is loaded from a CSV file.


**-Preprocessing:**

The code preprocesses the data by splitting the text into sentences and annotating the named entities. The SentenceGetter class is used to do this. It also converts the text and labeled entities into numerical representations.

**-Model Architecture:**

The model architecture consists of an Embedding layer, an LSTM layer with 100 units, and a Dense layer with softmax activation. The model is compiled with the Adam optimizer and categorical cross-entropy loss.

**-Training:**

The model is trained using the fit method of the Sequential class. The training data is split into training and testing sets using the train_test_split method from the sklearn.model_selection module. The fit method is called with a batch size of 32 and for 5 epochs. The training and validation accuracy and loss are recorded and plotted.

**-Evaluation:**

The model is evaluated on the testing set using the evaluate method of the Sequential class. The test loss and accuracy are printed to the console.

**-Results:**

The model achieves an accuracy of **98.84%** on the testing set after 5 epochs of training.
