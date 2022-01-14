### README

The easiest way to use the code is to put the needed files(weight files, model files etc.) in to your Google Drive, open the Colaboratory notebook, connect the notebook with the Drive, adapt file paths and then start exploring.

In order to use the full extent of the code you need to put the "Fonts" folder (located in  "Google_Drive_files") into your Google Drive. 

To use the code to train a model, replace the "### model ###" part in the "lstm_ocr" notebook  accordingly with your desired model architecture from the appropriate ".txt" file content. 

To test a model, replace the "### model ###" part in the "test_lstm_ocr" notebook  accordingly with your desired model architecture from the appropriate ".txt" file content.
You also need to put the folder "weights" (located in "Google_Drive_files") into your Google Drive. Use the ".h5" files to load weights into the model architecture in question.
The "e{number}" signifies the number of epochs the model (here weights) was trained for.
To test the models on real data (images of actual handwriting), use the folder "real_words" in the "images" folder. Put the folder into your Google Drive, adjust the file paths in "test_lstm_ocr" if needed.


# Files 

".ipynb": Google Colaboratory Notebook(Jupyter Notebook) containing Python code. Should be run using Google Colaboratory.

".h5": Contains multidimensional scientific data. Is either a fully saved model including weights or just a model's weights. Note that loading foreign weights into the wrong model will raise errors.
Full models are saved using the full name of the model architecture as such: "<model_architecture>.h5"
Weights are saved using either a date stamp or a file name incorporating the word "weights".

".txt": Simple text file. Contains code needed to recreate models to train or test them. 

"model.png": Visualization of the model architecture. Created using a Keras function. Also displays input-output sizes.

"final_test_{}.png": Visual representation of the final test result/prediction.