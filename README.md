
# Accent-Aware Speech Recognition System 🎙️

A deep learning-based Automatic Speech Recognition (ASR) system that adapts to diverse English accents using speaker adaptation techniques, signal processing, and transfer learning.

---

## 🧠 Project Overview

Many speech recognition systems perform poorly in multi-accent environments due to bias toward standard dialects. This project tackles that challenge by:

- Using **CNNs** and **RNNs/LSTMs** for feature extraction and sequence modeling
- Implementing **MLLR** (Maximum Likelihood Linear Regression) for speaker adaptation
- Enhancing model generalization with **data augmentation** techniques like pitch shifting and noise injection

---

## 📊 Business Use Cases

- **Transcription Services**: Automate accurate transcription for multi-speaker recordings
- **Accessibility Tools**: Provide real-time captioning for hearing-impaired users
- **Customer Support**: Improve voice bot recognition across regional accents
- **Virtual Assistants**: Better interpret voice commands in smart devices
- **Language Learning**: Offer accent-aware pronunciation feedback

---

## 📁 Project Structure

```
Accent-Aware-ASR/
├── 1_Cleaned_Data/              # Processed and labeled audio + metadata
├── 2_Code_Scripts/              # Python scripts for preprocessing, training, EDA
├── 3_Trained_Models/            # Saved models and checkpoints
├── 4_Reports/                   # Evaluation results and metrics
├── 5_PowerBI_Dashboard/         # CSVs for Power BI visuals
├── 6_GUI_or_API/                # Optional interface or deployment
├── README.md
```

---

## 🛠️ Key Features

- ✅ Accent-tagged voice data (Common Voice v21.0)
- ✅ Audio preprocessing (resampling, normalization, chunking)
- ✅ Data augmentation (pitch shift, noise injection)
- ✅ Spectrogram-based CNN feature extraction
- ✅ Fine-tuning with pre-trained Wav2Vec2
- ✅ MLLR-based speaker adaptation with Kaldi
- ✅ Accuracy, WER, and latency evaluation
- ✅ Power BI dashboards for analysis

---

## 📦 Dependencies

- Python 3.8+
- `librosa`, `soundfile`, `pandas`, `tqdm`, `matplotlib`, `seaborn`
- `transformers`, `jiwer`, `torch`, `tensorflow`
- [Kaldi](https://kaldi-asr.org/) (for MLLR adaptation)
- Power BI (for visualization)

---

## 🚀 Getting Started

### 1. Preprocess Data
```bash
python scripts/preprocess_audio.py
```

### 2. Train ASR Model
```bash
python scripts/train_model.py
```

### 3. Evaluate with WER
```bash
python scripts/evaluate_model.py
```

---

## 📈 Evaluation Metrics

| Metric        | Description                          |
|---------------|--------------------------------------|
| **WER**       | Word Error Rate                      |
| **Accuracy**  | Correct recognition rate by accent   |
| **Latency**   | Time from audio input to transcript  |
| **Perplexity**| Language model prediction confidence |

---

## 📊 Power BI Dashboards

- Accuracy heatmaps by accent
- WER before/after adaptation
- Phoneme distribution
- Confusion matrix for misrecognitions

---

## 🔍 Insights & Results

- WER improved up to **7.5%** after MLLR adaptation for Indian and British English
- Significant reduction in bias toward standard accents
- Real-time capable processing for user interaction

---

## 📚 References

- Mozilla Common Voice Dataset v21.0  
  [https://commonvoice.mozilla.org/en/datasets](https://commonvoice.mozilla.org/en/datasets)

---

## 📌 License

This project is licensed under the MIT License.
