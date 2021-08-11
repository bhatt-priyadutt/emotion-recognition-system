# emotion-recognition-system
1.) Data Loading:
* Dataset(metadata) for the audio files was loaded using pandas "read_csv()" function.
* Loading the audio train files was done by the package "Librosa" using "load()" function.

2.) Extract Features:
* Extracting features, here we will be using Mel-Frequency Cepstral Coefficients(MFCC) from the audio samples. 
* The MFCC summarises the frequency distribution across the window size, so it is possible to analyse both the frequency and time characteristics of the sound. 
* Also, with MFCC, I also used other information of audio files that are: Spectral Centroid, Spectral Rolloff, Spectral Bandwidth, Zero-Crossing Rate.
* These audio representations will allow us to identify features for classification.

3.) Encoding categorical feature:
* Using Labelencoder to convert the emotion(Dependent) feature into categorical(0 0 0 0 0 0 1) in order to feed it into the ANN(Artifical Neural Network).
* At the end, we can inverse transform the categorical binary values to get the feature value back for the results.

4.) Feature Scaling:
* Using Standard scaler, normalized the values of independent features.

5.) Over-Sampling:
* Used Synthetic Minority Oversampling Technique(SMOTE) for balancing the dataset.

6.) Model Building:
* Used Tensorflow Artificial Neural Network(ANN) model.
* Model accuracy - 99%

<img src="https://github.com/bhatt-priyadutt/priyadutt-portfolio/blob/main/images/emotion.png" />

7.) Testing:
* Used the same procedure for extracting the features of audio files for test data.

