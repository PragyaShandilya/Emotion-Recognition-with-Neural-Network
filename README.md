# Emotion-Recognition-with-Neural-Network

## Problem Statement
To develop an accurate speech sentiment recognition model that can classify spoken emotions into predefined categories (e.g., happy, sad, angry, neutral) using machine learning techniques.

## Overview 
1. This model is built to recognize emotions based on  the Toronto Emotional Speech Set which has been divided into 80% training dataset and 20% testing dataset. Following are the emotions available in the dataset:
   - Happy
   - Sad
   - Angry
   - Fear
   - Neutral
   - Disgust
   - Pleasant Surprise  
2. I have used waveform plots and spectograms for the purpose of data visualisation, along with a histogram to depict the distribution of the dataset.
3. I extracted Mel-frequency cepstral coefficients (MFCCs) to be used as features.
4. The model,  used was a sequential neural network with total of 8 layers: 1 LSTM layer, 4 dropout layers and 4 dense layers.
   - The LSTM layer consisted of 256 neurons.
   - The input shape was 40,1 because 40 MFCC extracted for one emotion/label.
   - 50 epochs were used and for each iteration 50% of neurons were dropped to avoid overfitting.
   - The output layer has 7 neurons, one for each possible emotion.
  
## PROJECT 
### Dataset 
1. It consists of 200 words said by 2 different actresses of age 26 and 64. Each word has been said in all the 7 emotions.
   - ![image](https://github.com/user-attachments/assets/4a91ca60-4cc6-451d-8520-e2f4a204b097)

2. Examples of Data visualisation
   - ![image](https://github.com/user-attachments/assets/d18a1809-bc20-4558-b886-a3c42ea81cfd)

3. Feature Extraction - 1D array of 40 MFCC calculated for each audio file
   - ![image](https://github.com/user-attachments/assets/76f54820-925f-44ac-9d9e-260f1573ea43)
   
4. Accuracy
   Average Training accuracy was 96.73% and Average Testing accuracy was 92.59%
   


## Notes and Relevant Links
 This project has been inspired from - https://github.com/x4nth055/emotion-recognition-using-speech
 Dataset Link - https://www.kaggle.com/datasets/ejlok1/toronto-emotional-speech-set-tess
