# Automatic Speech Recognition with PyTorch

This repository contains the code for a deep learning model built with PyTorch to perform Automatic Speech Recognition (ASR). The model is designed to convert audio speech clips into text transcriptions using a stacked Long Short-Term Memory (LSTM) architecture.

---

## Key Features

- **Model**: A deep learning model implemented with stacked, bidirectional LSTM layers.
- **Feature Extraction**: Converts raw audio waveforms into Mel-Frequency Cepstral Coefficients (MFCCs) for model input.
- **Framework**: Built entirely using PyTorch and the `torchaudio` library for audio processing.
- **Dataset**: Trained and evaluated on the LJ Speech Dataset, which consists of approximately 24 hours of English speech from a single speaker.

---

## Model Performance

The model was trained and tuned to achieve accurate transcription. The final performance was measured using standard ASR metrics:

| Metric | Score |
| :--- | :--- |
| **Word Error Rate (WER)** | **12%** |
| **Character Error Rate (CER)** | **8%** |

*Lower scores indicate better performance.*

---

## Dataset

The model was trained on the **LJ Speech Dataset**. This dataset is in the public domain and is available for download on Kaggle:

- **Link**: [https://www.kaggle.com/datasets/mathurinache/the-lj-speech-dataset](https://www.kaggle.com/datasets/mathurinache/the-lj-speech-dataset)

---

## Technologies Used

- Python
- PyTorch
- torchaudio
- jiwer (for WER/CER calculation)
- pandas
- kagglehub

---

## Usage

To run this project, follow these steps.

1.  **Clone the repository:**
    ```sh
    git clone [https://github.com/mehta-sahil/speech-recognition.git](https://github.com/mehta-sahil/speech-recognition.git)
    cd speech-recognition
    ```

2.  **Install the required libraries:**
    It is recommended to create a virtual environment first.
    ```sh
    pip install -r requirements.txt
    ```

3.  **Run the training script:**
    ```sh
    python your_script_name.py
    ```
    The script will automatically download the LJ Speech dataset via the `kagglehub` library and begin the training and evaluation process.
