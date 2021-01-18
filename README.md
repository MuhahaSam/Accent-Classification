# Accent-Classification
This project is about creating NN, witch coud recognize accent in english speaking 
The source of data is from https://www.kaggle.com/rtatman/speech-accent-archive.

The main idea of automation speech accent recognition is spliting audio file in to a multiple finished phrase.
It could be end of setence or word, but the point is separation should not happen in the middle of word.
For solving this task i used the sliding window algorithm. If values of absolute mean of amplitudes in window is under threshold, than it signals abount silence, that means 
end of phrase(New_data_cutting.ipynb). 



After spliting the audio files, i transformed each splited audio file in to a spectograms (spectogramm.ipynb).

The last step in designing the CNN model for training on the spectograms (CNN.ipynb). 

