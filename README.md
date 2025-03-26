Using python, meadiapipe and opencv we were able to analyse data from the webcam and also identify landmarks on the hand that can be used to create datasets of x and y coordinates. Using these datasets,we trained a random forest classifier using scikit-learn to create a sign language model. Putting it all together, the model can be used in real time in conjuction with opencv to detect hand signs.

Dataset can be downloaded from:
https://www.kaggle.com/datasets/ayuraj/asl-dataset

How to try it out
1. Pull the project/Download a zip and open in an IDE of your choice
2. Run the files in the order
3. collect_imgs (Follow the steps on screen to collect images)
4. create_dataset
5. train_classifier (This should reveal the classifier score in the console)
6. test_classifier (Final file that should run the model in real time)We trained it on 100 images for each letter of the alphabet (36 classes for 26 letters+10 for digits). The labeling process for each image ensured that the model could accurately recognize each sign language letter during a video, even with variations in hand shape and movement.
   
-----> In the real-time detection phase:
1. Start Webcam Feed: Launch the real-time detection script.
2. Perform Gestures: Perform the ASL gestures in front of the webcam.
3. View Predictions: See the predicted gesture and probability visualization on the screen.
4. The webcam feed is processed frame by frame.
5. Key points are extracted and fed into the trained model.
6. The model predicts the gesture being performed.
7. The predicted gesture is displayed on the screen, along with a visualization of prediction probabilities.Here are few snippets representing real time detection performed

<img src="https://github.com/user-attachments/assets/c3645eb3-c77c-4ed4-ab93-f95d3565bbeb" width="300"/>
<img src="https://github.com/user-attachments/assets/6149cdb8-23c3-4896-b211-fca17d0ce8c1" width="300"/>
<img src="https://github.com/user-attachments/assets/895dc1f7-5cf0-4da2-a21b-f1f3b00959c7" width="300"/>
<img src="https://github.com/user-attachments/assets/562cdc13-381a-4098-b5dd-8e70a3f566c0" width="300"/>
<img src="https://github.com/user-attachments/assets/49ce352a-9344-4f83-8ce1-1e7256b77527" width="300"/>
<img src="https://github.com/user-attachments/assets/142a8c35-cadf-4919-b38f-a6363574e463" width="300"/>
<img src="https://github.com/user-attachments/assets/22e9e4b8-0af9-4647-88d1-084b81221b08" width="300"/>
<img src="https://github.com/user-attachments/assets/b0a3ccb4-8d7f-4f11-94d6-77ee6e272496" width="300"/>
<img src="https://github.com/user-attachments/assets/5e049796-ab37-4757-94bc-f77558f252d3" width="300"/>
<img src="https://github.com/user-attachments/assets/83f9746c-4975-4010-b1d9-51bb6b35d8a5" width="300"/>
<img src="https://github.com/user-attachments/assets/316026e5-5ea7-480b-beb5-6c880e38b2aa" width="300"/>
<img src="https://github.com/user-attachments/assets/579d8ef1-c692-492f-ace9-43a5ae4cc6a2" width="300"/>
<img src="https://github.com/user-attachments/assets/1b8a4a9f-ff53-4ed6-bfd7-bd8e633a6131" width="300"/>
<img src="https://github.com/user-attachments/assets/b888c98b-017d-433f-808f-826be1b74128" width="300"/>
<img src="https://github.com/user-attachments/assets/df0ed0fc-115e-4b7e-a222-d8643d2b14d2" width="300"/>
<img src="https://github.com/user-attachments/assets/7b28a584-f407-4530-b0da-da8bb6cb15c1" width="300"/>
<img src="https://github.com/user-attachments/assets/4b9c2c15-c1ea-4812-b0f5-27d454cfff69" width="300"/>
<img src="https://github.com/user-attachments/assets/52dd5d1a-0ea7-49d5-8d5d-b15791790920" width="300"/>
<img src="https://github.com/user-attachments/assets/aac40d44-0c4e-43b6-80ba-9eff9edf03bf" width="300"/>
<img src="https://github.com/user-attachments/assets/226c0cd9-770c-4067-8301-fdaa76cbfd64" width="300"/>
<img src="https://github.com/user-attachments/assets/8669dc66-d299-4ce7-8f8b-032f03849ca5" width="300"/>
<img src="https://github.com/user-attachments/assets/4a34ebc7-e4c2-4400-a723-a0b2f24ea3c2" width="300"/>
<img src="https://github.com/user-attachments/assets/412923b1-1c51-4216-b42b-4ee75d97b4e3" width="300"/>
<img src="https://github.com/user-attachments/assets/dd98cdbd-178e-431a-9732-78452a50cd34" width="300"/>
<img src="https://github.com/user-attachments/assets/0cc0b2a5-fa5a-495a-b7ba-22b66ebcc49c" width="300"/>
<img src="https://github.com/user-attachments/assets/2af316c3-3a1c-462c-be5a-5074f796173e" width="300"/>
