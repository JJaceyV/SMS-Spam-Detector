# SMS-Spam-Detector
## Credit
I took a lot of inspiration from Mariya Sha to build up this Python GUI. My GUI is the updated version from her instruction since the syntax of Dearpygui in her video is no longer valid. Please visit her github site and YouTube videos for more details. You can also refer to the latest documentation of dearpygui library for better understanding and personal customization. All the links that I used as resources when doing this project will be enclosed down here
  - Github: https://github.com/MariyaSha/SimpleSMSspamFilter_GUI/blob/main/finishedProject/app.py
  - Youtube: https://www.youtube.com/watch?v=2RocXKPPx4o
  - Dearpygui documentation: https://dearpygui.readthedocs.io/en/latest/


## Summary
The goal of this project is to build a GUI to collect users' inputs and then return the prediction based on the built-in SVM model. app.py is the file where I designed the graphic user interface and the functions.py is where I built the SVM model

## Further explanation of what I have done in each file
functions.py
  - In this file, I utilized natural language processing techniques to process the texts in the dataset. This included:
      - Drop unnecessary columns
      - Drop duplicate values
      - Apply Label Encoder on the target values
      - Remove the stopwords and meaningless characters to avoid noises
      - Lemmatize the texts
  - After cleaning the texts, I had them vectorized by using a simple technique called Count Vectorizer
  - Finally, I built the SVM model using the sklearn library and created a predict function

app.py
  - Here I resized the window and viewport of the GUI to the size I preferred
  - I uploaded the image that I wanted to show in the app
  - I created all the necessary buttons and text boxes and adjusted them so that they fit in with the arrangement of the app
  - I made some other format adjustments towards the buttons, texts, and the window. Eventually, I imported the functions that I had created in the functions.py file to connect the GUI with the built-in model. Voila the GUI was finished

## How does the GUI work?
To see how the GUI looks like and how it works, please click the link below: 
  - 

## Some drawbacks of this project
- Instead of using SVM model to detect spam messages, you can try some deep learning models like LSTM, BERT,... for comparison and better predicted results.
- The vectorization resolution in this project is quite simple, you can try some neural network related techniques like word2vec or glove to see if there are any improvements on the final outcomes

## Find a bug?
If you found an issue or would like to submit an improvement to this project, please don't hesitate to pull a request
