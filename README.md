# ASR-using-CNN
Automatic speech recognition using Convolutional Neural Networks
A total of 9 folders are being utilised in this script, namely: 84, 174, 251, ASR_Model, Audio_Data, N_Data, New_Data, test_data, and Test_Data.

There are two datasets involved, and each dataset is treated and processed to get a resulting dataset. 
We are using audio datasets as inputs and then converting their audio samples into audio spectrographs.

1. Starting at the first dataset, it is more of a passage type dataset for testing transcription accuracies.
-> It is present in the 3 folders named: 84, 174, and 251.
-> Each folder has more than folder in itself, and inside them there are audio samples, and a transcription in a singular text file.
-> This data was not used to build a convolutional neural network, as it needs a dictionary of words to be built around it.
-> This data was present in "flac" files.

2. Second Dataset consists of words, in particular 3 of them: "bed", "cat", and "happy". 
-> We have samples consisting of the same word said in different enunciations, and different people, for each of these 3 words.
-> We use classification algorithm to determine between these words.
-> The dataset is originally present in "wav" files.
-> The folder "Audio_Data" contains the training data.
-> The folder "test_data" contains the test data sample.
-> The link from where it was acquired is "https://github.com/lukas/ml-class/tree/master/videos/cnn-audio/data". There is a lot more of it there.

3. Both these datasets were loaded using "os" package from python and each file was loaded in memory converte to image, and saved again.
-> Then the files were loaded again, and processing was done.
-> This time these spectrographs were loaded into a set of convolutional networks, one with one convolutional layer, the other with two.
-> Finally, the test data was made to go through the same process, where its "Test_Data" folder was used to house Spectrographs.
-> And "model.predict" used to find the predicted class.


Where, New_Data contains spectrographs for First "flac" dataset, and the N_Data contains spectrographs for the Second "wav" words dataset.
And last but not the least, ASR_Model folder contains the two tensorflow models.
