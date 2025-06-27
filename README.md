# 🎤 Human Emotion Detection from Voice

This project detects human emotions using voice input. It uses audio processing and machine learning techniques to classify emotions such as happy, sad, angry, calm, and more.

## 📌 Objective

To build a machine learning model that detects emotions from speech and provides a simple Streamlit web interface for users to interact and test.

## 📚 Dataset

- **RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)**  
  The dataset contains 1440 `.wav` audio files representing 8 different emotions.

## 🛠️ Tools & Libraries Used

- Python
- NumPy, Pandas, Matplotlib, Seaborn
- Librosa (Audio processing)
- Scikit-learn (Model training)
- Joblib (Model serialization)
- Streamlit (Web interface)

## 🚀 Steps Involved

1. **Data Preparation**
   - Copy `.wav` files from RAVDESS into `emotions_dataset/`
   - Extract labels from filenames

2. **Feature Extraction**
   - Use Librosa to extract MFCC, Chroma, and Mel Spectrogram features from audio

3. **Model Training**
   - Train a Random Forest Classifier on extracted features
   - Evaluate with confusion matrix and classification report

4. **Model Saving**
   - Save trained model using `joblib` in `model/` folder

5. **Streamlit Web App**
   - Build UI to upload audio file
   - Predict and display emotion
   - Show optional emotion trend graph
   - Save prediction history/session data
  
  ## 🔧 Installation

### 🔗 Clone the repo
```bash
git clone https://github.com/kalyani-ch123/Emotion-Voice-Detection.git
cd Emotion-Voice-Detection

**💡 Create a virtual environment (optional)**

python3 -m venv venv
source venv/bin/activate

**📦 Install dependencies**

pip install -r requirements.txt

**🚀 Run the App**

streamlit run app.py
Then, open your browser to: http://localhost:8501

**🧪 Model Performance**
Metric	Value
Accuracy	~85-90%
Classifier	SVM / RF
Dataset	RAVDESS
Sample Size	1440 Audio Files
📈 You can retrain the model using the training notebook provided.

**📂 Folder Structure**

Emotion-Voice-Detection/
├── data/                # Audio samples (optional)
├── models/              # Trained model (pkl)
├── app.py               # Streamlit UI
├── feature_extractor.py # Feature functions
├── train_model.py       # ML training script
├── requirements.txt
└── README.md

**✨ Future Enhancements**

    🎙️ Real-time voice recording in the browser

    🤖 Deep learning models (LSTM, CNN, wav2vec2)

    🌐 Deploy to HuggingFace or Streamlit Cloud

    📈 Emotion trends chart across multiple recordings

    🔄 Multilingual emotion detection

**💬 Feedback**

Found a bug or want to suggest a feature? Feel free to open an issue or a pull request!

    🌟 Star the repo if you like it. It motivates me to build more! 😊



