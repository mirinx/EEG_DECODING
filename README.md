#  EEG Decoding Prototype: Motor Imagery Classification
A high-accuracy (94.83%) BCI prototype designed to decode brain signals for digital avatar control. This project utilizes Common Spatial Patterns (CSP) and Linear Discriminant Analysis (LDA) to classify Motor Imagery (Left vs. Right hand).

##  The Vision: From Rehabilitation to Full-Dive
Inspired by the **Full-Dive technology** from *Sword Art Online (SAO)*, this project serves as my foundational step toward bridging the gap between human neural signals and digital environments. 

My goal is to develop BCI systems that empower users with physical limitations, such as stroke or paralyzed patients, to regain freedom in a 3D world.
* **Neural Rehabilitation:** Using motor imagery to trigger neuroplasticity, turning "thoughts" into a form of physical therapy.
* **Restoring Interaction:** Enabling communication and movement through digital avatars for those with limited physical mobility.

##  Project Overview
This prototype decodes brain signals (EEG) to distinguish between **Left Hand** and **Right Hand** motor imagery. This decoding logic will serve as the "Brain" for my future 3D bone-model control project in Blender/Unity.

### **Technical Stack**
* **Language:** Python 3.x
* **Environment:** Google Colab / MNE-Python
* **Dataset:** BCI Competition IV 2a (Standardized via MOABB)
* **Libraries:** `mne`, `moabb`, `scikit-learn`, `numpy`

##  The Pipeline
1. **Data Acquisition:** Accessing standardized Motor Imagery datasets (Left vs. Right hand).
2. **Preprocessing:** Applied an **8-30 Hz Band-pass filter** to isolate Mu and Beta rhythms while removing low-frequency artifacts.
3. **Feature Extraction:** Utilized **Common Spatial Patterns (CSP)** to maximize signal variance between classes.
4. **Classification:** Applied **Linear Discriminant Analysis (LDA)** to establish a robust decision boundary.

##  Results
* **Highest Accuracy: 94.83%**
* **Configuration:** `n_components=6` for CSP spatial filtering.

This high accuracy demonstrates that the decoder is stable and ready for real-time system integration.

##  Project Roadmap
[x] Phase 1: Foundation & Baseline Decoding(current)
[ ] Phase 2: Deep Learning & Real-time 3D Integration
[ ] Phase 3: Multi-Action & Multi-Class Expansion


