# Libras Alphabet Transcriber


## :bulb: Inspiration

LIBRAS stands for "_Língua Brasileira de Sinais_", translating to **Brazilian Sign Language** in English. It serves as the primary mode of communication for millions of deaf individuals in Brazil.

The development of a Libras Alphabet Transcriber in real-time using Machine Learning is crucial for promoting inclusivity and enhancing accessibility for the deaf community in Brazil. 
While numerous projects have focused on American Sign Language (ASL), there is a noticeable gap in the availability of tools specifically tailored to Libras.

The application provides educational advantages by creating inclusive learning environments for students who are deaf or hard of hearing, as well as for individuals interested on learning Libras.

Leveraging technology to bridge the communication gap is essential for creating a more inclusive society :blush:

This project was made for AI4GOOD [Brazil Conference](https://www.brazilconference.org/) at Harvard & MIT 2024

## :computer: What it does

![Example](https://gizmodo.uol.com.br/wp-content/blogs.dir/8/files/2021/02/nyan-cat-1.gif)


The Libras Alphabet Transcriber is a Python program that employs Computer Vision and Machine Learning techniques to recognize and transcribe gestures of the Brazilian Sign Language (LIBRAS)
alphabet in real-time using your webcam. The program utilizes a Hand Tracking module to detect hand landmarks, and, based on their coordinates, employs a machine learning algorithm 
to classify and transcribe the corresponding sign language alphabet.

### :gear: Available Machine Learning Models
- KNN [default]
- Random Forest
- SVM
- Logistic Regression
- Neural Network


## :hammer: How we built it
1. Creation of a Libras static alphabet dataset
   - Refer to the [./dataset](./dataset) folder for more information about the data format
2. Train different models using [scikit-learn](https://scikit-learn.org/stable) and [Keras](https://keras.io/)
   - Check [train.ipynb](train.ipynb) for training results 
3. Real-time transcriber
   1. Open your webcam
   2. Obtain hand positions using the [CVZone](https://github.com/cvzone/cvzone) Hand Tracking Module
   3. Normalize and reshape hand landmark coordinates 
   4. Make predictions using a selected model
   5. Display results in an [OpenCV](https://opencv.org/) window


## :camera: Usage
- Hold the same sign for 10 frames to write it

- Use this sign :hand: for spacebar

```bash
# clone the repository
git clone https://github.com/victor-nasc/LIBRAS-Recognition.git

# install dependencies
pip install -r requirements.txt

# Run the program
python3 main.py
```

## Authors
Victor Nascimento Ribeiro - [LinkedIn](https://www.linkedin.com/in/your-linkedin-profile/)

Gustavo Vaz Pinto - [LinkedIn](https://www.linkedin.com/in/your-linkedin-profile/)

Eduardo Cruz Guedes - [LinkedIn](https://www.linkedin.com/in/your-linkedin-profile/)

