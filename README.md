# Gait Analysis using CASIA-B Dataset

This project focuses on **recognizing individuals based on their gait silhouettes** using deep learning. We leverage a combination of **CNN** for feature extraction and **BiLSTM** for sequence modeling to classify gait patterns.

## 📁 Dataset

**Source:** [CASIA-B Dataset on Kaggle](https://www.kaggle.com/datasets/trnquanghuyn/casia-b)

### Dataset Structure

The CASIA-B dataset is organized as follows:

- **Main folder (`output/`)** contains **124 subfolders**, each representing a unique individual (label/object) — totaling **124 subjects**.
- Each subject folder contains three condition-based subfolders:
  - `nm` — normal walking
  - `bg` — walking with a bag
  - `cl` — walking with a coat
- Each of these subfolders contains multiple **view-angle subfolders** (e.g., `000`, `018`, `036`, etc.), representing the **angle** at which the silhouette was captured.
- Finally, each angle folder contains a **sequence of silhouette images** representing the gait cycle of that individual.

- ![image](https://github.com/user-attachments/assets/9ebd1bd2-57b3-4cf4-ab38-484be56f14e7)


## 🧠 Model Architecture

The model follows a two-stage deep learning pipeline:

1. **CNN (Convolutional Neural Network):**
   - Extracts spatial features from each silhouette image.
   - Captures the posture and contour of the person in each frame.

2. **BiLSTM (Bidirectional Long Short-Term Memory):**
   - Processes the sequence of features extracted from the silhouettes.
   - Learns the temporal dynamics and order of movement in gait sequences.

This combination allows the model to understand both the **individual frame features** and the **motion pattern over time**, which are critical for accurate gait recognition.

## 🎯 Objective

Our goal is to **identify or verify a person based solely on their gait silhouette**, which can be useful in:

- Surveillance systems
- Biometric security
- Healthcare and rehabilitation

## 🛠️ Technologies Used

- Python
- TensorFlow / Keras
- NumPy, OpenCV
- Matplotlib, Seaborn (for visualization)

## 🚧 Project Status

- ✅ Dataset preprocessing completed
- ✅ videos to silhouettes sequnce conversion 
- ✅ CNN feature extractor implemented
- ✅ BiLSTM sequence model integrated
- ⏳ Training and evaluation in progress

## 📬 Contact

For any queries or collaboration interests, feel free to reach out.

---

