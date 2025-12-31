#  EEG Decoding Prototype: Motor Imagery Classification
A high-accuracy (94.83%) BCI prototype designed to decode brain signals for digital avatar control. This project utilizes Common Spatial Patterns (CSP) and Linear Discriminant Analysis (LDA) to classify Motor Imagery (Left vs. Right hand).

##  The Vision: From Rehabilitation to Full-Dive
Inspired by the **Full-Dive technology** from *Sword Art Online (SAO)*, this project serves as my foundational step toward bridging the gap between human neural signals and digital environments. 

My goal is to develop BCI systems that empower users with physical limitations, such as stroke or paralyzed patients, to regain freedom in a 3D world.
* **Neural Rehabilitation:** Using motor imagery to trigger neuroplasticity, turning "thoughts" into a form of physical therapy.
* **Restoring Interaction:** Enabling communication and movement through digital avatars for those with limited physical mobility.

##  Project Overview
This prototype serves as a high-precision neural decoder, achieving 94.83% accuracy in classifying Left Hand and Right Hand motor imagery.

Beyond simple classification, this logic functions as the "Neural Core" (The Brain) for an integrated BCI system. It is designed to bridge raw neural oscillations with digital execution, providing the foundational control layer for:
**Real-time 3D Avatar Control:** Directly driving skeletal transforms in Blender/Unity.
**Neuro-rehabilitation:** Facilitating the recovery of stroke patients through intentional movement visualization.

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
*[x] Phase 1: Foundation & Baseline Decoding(current)*<br>
[ ] Phase 2: Deep Learning & Real-time 3D Integration<br>
[ ] Phase 3: Multi-Action & Multi-Class Expansion


