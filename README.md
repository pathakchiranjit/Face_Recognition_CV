### Capstone Group Project (GCDAI) - **Consulting Assignments** **Face_Recognition_CV**

<img src="https://github.com/pathakchiranjit/Face_Recognition_CV/blob/main/Snaps/1.png?raw=true" align='left'><br/>


The client for this project is the Administration Department at **AutoBox** having over a thousand employees.

They want to maintain a **central database** of all of their employees.
And, extra emphasis is on **increasing security** and ease of operation.
The idea is to create a **web-based app for Facial Recognition** in order to have rightful entry to the office premises and restrict any trespassers.
Once the employees are identified on a daily basis, they can have a simple entry and exit procedure without any manual intervention.They want to deal with their existing employee’s database and those coming in as a new recruit.

**Current Practice:**

The existing employees or the ones joining the Company gets a card having a QR(RFID) code with unique identification for entry and exit.

**The current practice suffers from the following problems:**

- This approach is too haphazard. The quality of **insight gained is misaligned** due to misleading data.
- The second problem is these **insights can't be aggregated** to frame certain policies on this.
- The third problem is the **security breach of the Company**, which can hamper the situation very badly.

As a part of the **digital approach**, the Admin Department hires **INSAIDians** as their **AI consultant** in order to supplement their security protocols with a more proactive approach.



### **Weekly Goals for the team?**:
The AI consultant team will follow the below week-wise goals,

<img src="https://github.com/pathakchiranjit/Face_Recognition_CV/blob/main/Snaps/3.png?raw=true" align='left'><br/>































## Table of Contents

1. [Objective: Problem Statement](#section1)<br>
2. [Tools : Importing Packages, Libraries & Defining Functions:](#section2)<br>
  - 2.1 [Import Packages and Libraries:](#section201)<br>
  - 2.2 [Defining Functions :](#section202)<br>
    - 2.2.1 [big_bbox : To find bigger bounding box as title face for an image having multiple faces.](#section2021)<br>
    - 2.2.2 [extract_face : Pipe line containing image preprocessing steps as convert to 'RGB' --> detect faces --> identify bigger bounding box as target face --> extract the face --> crop to required dimension for embedding model.](#section2022)<br>
    - 2.2.3 [load_faces : extract faces for images in a folder](#section2023)<br>
    - 2.2.4 [load_dataset : extract faces for images of all the sub-folder in a directory and add label the image as per the sub-folder name](#section2024)<br>
    - 2.2.5 [get_embeddig : using a face embedding model and saved extracted faces the faces are being embedded](#section2025)<br>
    - 2.2.6 [load_faces_test : preprocess all the unseen/test images provided in a folder and returns the extracted faces, its embeddings and the name of the file](#section2026)<br>
    - 2.2.7 [proba : it will define whether final prediction is being 'Permitted' or 'Restricted' based on class probability threshold](#section2027)<br>
3. [Collecting & Loading Data](#section3)<br>
  - 3.1 [ Import train & validation dataset from G-Drive:](#section301)<br>
  - 3.2 [ Import unseen / test dataset from G-Drive:](#section302)<br>
4. [Data Preprocessing](#section4)<br>
  - 4.1 [Basic preprocessing: conversion to RGB and extraction of faces](#section401)<br>
  - 4.2 [Prepare Train and validation data set](#section402)<br>
  - 4.3 [Create Face Embeddings for Train and validation dataset](#section403)<br>
  - 4.4 [Perform Face Classification:](#section404)<br>
  - 4.5 [Random Checks for dataset:](#section405)<br>
5. [Prediction on Unseen data / Test data:](#section5)<br>
  - 5.1 [Preprocessing Pipeline: conversion to RGB, extraction of faces and get embeddings](#section501)<br>
  - 5.2 [Prediction with probability estimation using trained model](#section502)<br>
  - 5.3 [Prepare the submission file](#section503)<br>
6. [Conclusion](#section6)<br>
7. [Actionable Insights:](#section7)
8. [Limitation of the study:](#section8)
