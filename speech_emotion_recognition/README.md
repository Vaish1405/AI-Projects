
## 🗣️ Speech Emotion Recognition (SER) System

A deep learning-based project to detect human emotions from speech audio using Convolutional Neural Networks (CNN) and Long Short-Term Memory Networks (LSTM). Developed for COMP 569: Introduction to Artificial Intelligence.


## 📌 Project Overview

The system classifies audio inputs into emotional states such as:

    Happy 😊

    Sad 😢

    Angry 😠

    Fearful 😨

    Neutral 😐

    Disgust 🤢

    Surprised 😲

Use Cases:

    Mental health monitoring

    Human-computer interaction

    Security & forensics

    Emotion-aware virtual assistants

🧠 AI Techniques Used

    CNN: For spatial feature extraction from MFCCs

    LSTM: For capturing temporal dependencies in speech

    Improved LSTM: With batch normalization, dropout, and L2 regularization

🧪 Datasets

Trained and tested on four popular SER datasets:

    TESS: collected on the Northwestern University Auditory with a total of 2800 stimuli

    CREMA-D: from 48 male and 43 female actors from a variety of races and ethnicities

    SAVEE: 480 British English utterances in total

    RAVDESS: 12 female and 12 male professional actors speaking in a neutral North American accent

Standardized emotion labels were applied across all datasets.
⚙️ System Pipeline

    Preprocessing:

        Silence removal, normalization, noise filtering

        Feature extraction using MFCCs, delta MFCCs, chroma

    Model Training:

        CNN and LSTM models implemented in TensorFlow/Keras

        Random oversampling to handle class imbalance

    Evaluation:

        Accuracy, F1-score, confusion matrices

        Real-time loss/accuracy plots via TensorBoard

## 📊 Results

| Model         | Evaluation Accuracy | Test Accuracy |
| ------------- | ------------------- | ------------- |
| CNN           | 65.02%              | 65.40%        |
| LSTM          | 68.19%              | 66.63%        |
| Improved LSTM | **71.18%**          | **68.88%**    |


🛠️ Tools & Technologies

    Python, NumPy, Pandas

    TensorFlow / Keras

    Librosa (audio processing)

    Jupyter Notebooks

    Google Colab (GPU-accelerated training)

🚧 Challenges & Adaptations

    Class imbalance handled via oversampling

    Model overfitting reduced with dropout & early stopping

    Improved LSTM generalization through regularization and learning rate tuning

    Dataset harmonization across varied formats and labels