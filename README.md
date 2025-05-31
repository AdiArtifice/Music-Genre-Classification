Music Genre Classification with EfficientNetB0

A deep learning project to classify music genres using spectrogram images from the GTZAN Genre Collection and a transfer learning approach with EfficientNetB0.

📁 Dataset

Source: GTZAN Genre Collection

Processed & Split Dataset: Google Drive Folder - https://drive.google.com/drive/folders/1VWhWKcU9nbNqAeJVqn4iX-OnGJb07TSd?usp=sharing

Format: Spectrogram images generated from 30-second audio clips

Classes: 10 genres - Blues, Classical, Country, Disco, HipHop, Jazz, Metal, Pop, Reggae, Rock

Data Split: 80% Train / 10% Validation / 10% Test

🔧 Tools & Libraries Used

Python

TensorFlow & Keras (for model development)

EfficientNetB0 (pretrained CNN model)

Scikit-learn (for evaluation metrics)

Matplotlib (for plots and visualization)

Google Colab (development environment)

🚀 Project Workflow

Data Preparation

Converted audio to spectrogram images

Organized data in train/, val/, and test/ folders

Model Building

Loaded EfficientNetB0 (without top)

Added custom classification head

Compiled with Adam optimizer and categorical_crossentropy loss

Training

Trained with callbacks: EarlyStopping, ReduceLROnPlateau, ModelCheckpoint

Saved best model as .keras

Evaluation

Evaluated on test set

Generated confusion matrix and classification report

📊 Results

Test Accuracy: ~65%

Metrics: Precision, Recall, F1-score for all 10 genres

SAVED MODEL: https://drive.google.com/file/d/1N4n55QebQsVTb4gnA5nxiJ1crj0Ojvof/view?usp=sharing

📌 Key Learnings

How to use transfer learning with EfficientNet

Handling image datasets in Keras

Monitoring model performance with callbacks

Evaluating model using classification metrics and plots

🧠 Future Improvements

Apply data augmentation to improve generalization

Try different architectures (ResNet, Inception)

Add real-time music genre prediction with audio input

🙏 Acknowledgments

GTZAN Dataset by George Tzanetakis

EfficientNet by Google AI

Guidance & support by ChatGPT (OpenAI)

