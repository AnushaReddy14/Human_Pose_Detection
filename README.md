Human pose detection is an important task in computer vision with various applications such as fitness tracking, sports analysis, and rehabilitation. In this paper, I present a machine learning based approach for human pose detection. I used two datasets, a primary data set of yoga poses images and a Yoga-82 data set, to create a comprehensive data set of six target classes. Then employed the pretrained Mediapipe model for feature extraction and also employed under sampling and oversampling techniques to make the data balanced.

Used Support Vector Machine (SVM), Random Forest Classifier (RF), K-Nearest Neighbors (KNN) Classifier, Bagging Classifier, Gradient Boosting Classifier (GBC), and employed ensemble on various classifiers for classification task. Our approach achieves an accuracy of 92% using Ensemble methods and Support Vector Machine, demonstrating promising results for real-world applications of human pose detection.

To create a comprehensive dataset for human pose detection, we used two different datasets: the Yoga Image Classification dataset from Kaggle, and the Yoga-82 dataset. The Yoga Image Classification dataset, obtained from Kaggle, consisted of 107 directories of poses, while the Yoga-82 dataset was used to extract images of six poses not present in the Yoga Image Classification dataset through web scraping. The six target poses, namely Standing, Sitting, Reclining, Inverted, Balancing, and Wheel Poses, were selected for the study. Images of all other poses were grouped into their respective superclass categories.

The images from both datasets were preprocessed to remove any invalid file formats, and then we used the pre-trained Mediapipe pose detection model to extract the key features for each pose. This model detects 33 keypoints on a person's body and measure their visisbility.

Used the Mediapipe Pose Detection Model to extract key points and landmarks from images. Specifically, used the mppose library from Mediapipe to detect the poses in the images. This was done by processing the images and detecting the landmarks in each pose. Then drew the landmarks on a white background using the mpDraw library, and extracted the coordinates and visibility of each landmark. This information was then stored in a dataset in the form of a CSV file for further analysis.
Using the Mediapipe library provided us with an efficient and accurate way to detect and extract the pose information from images, which was essential for the study of classifying different human poses. Overall, the data collection and preprocessing process helped us to create a comprehensive and balanced dataset, which was used for our human pose detection study.

![Imbalance](https://github.com/AnushaReddy14/Human_Pose_Detection/assets/128181850/89928be3-d475-4802-afc2-a5c419ffef3b)
![Balanced](https://github.com/AnushaReddy14/Human_Pose_Detection/assets/128181850/189a54e6-c0e9-4495-8dec-126b4a53bc70)


This present a comparative study of different classification algorithms, namely K-Nearest Neighbor (KNN) Classifier, Random Forest Classifier, Support Vector Machine (SVM) Classifier, Bagging Classifier, and Gradient Boosting Classifier, and Ensemble method for combining the predictions of these algorithms. The aim of this study is to classify poses using the classification algorithms and evaluate the performance of these algorithms on a given dataset and determine which algorithm(s) perform best for this dataset.

![Picture1](https://github.com/AnushaReddy14/Human_Pose_Detection/assets/128181850/20b40e2c-87dc-4984-9876-0095a32576ce)

This implementation is able to handle real-time video processing with minimal latency. The SVM model enables the system to classify poses accurately and in real-time. It can also handle multiple people in the frame, although it will only classify the pose and detect the keypoints of a single person closest to the camera.
The real-time implementation of pose detection using Mediapipe and SVM classification provides an efficient and accurate solution for detecting human poses in real-time. The implementation has the potential to be utilized in various applications, such as fitness tracking, physiotherapy, and rehabilitation. The system's accuracy and efficiency make it a viable option for these applications, as it can detect poses accurately and in real-time.

![Sitting_pose](https://github.com/AnushaReddy14/Human_Pose_Detection/assets/128181850/823017d1-c292-4dfd-88e1-d5e2735370b7)
![Balancing_Pose](https://github.com/AnushaReddy14/Human_Pose_Detection/assets/128181850/c9d65545-8647-414f-bd47-1c06e395fd02)
![Reclining_Pose](https://github.com/AnushaReddy14/Human_Pose_Detection/assets/128181850/94d5a1be-7bb0-48d5-8827-de64c8c3ffa9)
![Sittingpose](https://github.com/AnushaReddy14/Human_Pose_Detection/assets/128181850/56b7d068-3149-4833-8e93-df04eebb0f23)

Our proposed human pose detection models have demonstrated high performance and robustness in detecting different target poses under various conditions. Utilized the Mediapipe library for landmark extraction and trained various machine learning models, including Support Vector Machines, Random Forest, Bagging, Gradient Boosting, and K-Nearest Neighbors, on the extracted landmarks to classify human poses.
However, it acknowledges that the accuracy of our models can be affected by factors such as image quality, lighting conditions, and occlusion. In particular, also observed limitations in the detection of pose landmarks in blurry images. Nonetheless, our results have shown the potential of our models.

