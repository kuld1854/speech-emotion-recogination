# Speech Emotion Recognition Project README

## Project Description

This project focuses on recognizing human emotions and states from speech. It utilizes the RAVDESS dataset (Ryerson Audio-Visual Database of Emotional Speech and Song) for training and testing. The dataset includes audio recordings with various emotional states.

### Data Description

The RAVDESS dataset includes audio files with filenames containing important information:

- Modality (01 = full-AV, 02 = video-only, 03 = audio-only).
- Vocal channel (01 = speech, 02 = song).
- Emotion (01 = neutral, 02 = calm, 03 = happy, 04 = sad, 05 = angry, 06 = fearful, 07 = disgust, 08 = surprised).
- Emotional intensity (01 = normal, 02 = strong).
- Statement used in the file for emotion depiction.
- Repetition (01 = 1st repetition, 02 = 2nd repetition).
- Actor (01 to 24, odd numbered actors are male, even numbered actors are female).

### Models Used

This project employs two models for emotion recognition:

1. **MLPClassifier (Multi-Layer Perceptron Classifier)**: This feedforward ANN model maps input data to appropriate outputs.
2. **CNN (Convolutional Neural Network)**: A 1D CNN is used to automatically learn spatial hierarchies of features from the audio data.

### Project Workflow

The project workflow includes the following steps:

1. Mounting Google Drive and unzipping the dataset.
2. Loading and visualizing audio files.
3. Extracting features using Librosa and Soundfile.
4. Splitting the dataset into training and testing sets.
5. Training the MLPClassifier model and optimizing hyperparameters using GridSearchCV.
6. Building and training a 1D CNN model for emotion recognition.
7. Saving and loading models.
8. Handling custom input for emotion recognition.

## Getting Started

### Prerequisites

Before running the code, make sure you have the following installed:

- Python
- Jupyter Notebook (optional but recommended)

### Installation

1. Clone this repository:

   ```
   git clone https://github.com/your-username/speech-emotion-recognition.git
   ```

2. Navigate to the project directory:

   ```
   cd speech-emotion-recognition
   ```

3. Install the required Python packages:

   ```
   pip install -r requirements.txt
   ```

## Usage

- **Training**: To train the models, run the provided Jupyter Notebook or Python scripts. Ensure you have the dataset properly set up.

- **Emotion Recognition**: You can use the trained models to recognize emotions from audio. Follow the provided code for inference or integrate the models into your applications.

## Custom Input

You can use the provided function `derive_data_custom` to process custom audio input for emotion recognition. Refer to the code for details.

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1. Fork the project.
2. Create your feature branch: `git checkout -b feature/new-feature`.
3. Commit your changes: `git commit -m 'Add new feature'`.
4. Push to the branch: `git push origin feature/new-feature`.
5. Submit a pull request.


## Acknowledgments

- The RAVDESS dataset authors for providing the emotional speech data.
- Librosa and Soundfile libraries for audio processing.
- TensorFlow and scikit-learn for machine learning.

## Contact

For any questions or feedback, please contact Kuldeep Chaudhary(mailto: kuld1854@gmail.com).
