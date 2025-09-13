Counterfeit Currency Detector (Indian Notes)

Identify fake vs genuine currency notes using classical image features and ML. This repo contains datasets, training/testing notebooks, a simple GUI prototype, and a detailed project report.

This was our mega-project on counterfeit note detection.

✨ Highlights

End-to-end notebook workflow (feature extraction → training → evaluation)

Experiments at two feature scales (≈500 and ≈2000 features) for comparison

Visual report with screenshots and confusion matrices

Prototype GUI notebooks to demo predictions

🗂 Project Structure
counterfeit_currency/
├─ 500_Features Dataset/           # images / features @ ~500 dims
├─ 2000_Features Dataset/          # images / features @ ~2000 dims
├─ 500_dataset/ and 2000_dataset/  # supporting data (features/labels)
├─ Fake Notes/                      # sample counterfeit images
├─ 500_Testing.ipynb               # eval notebook for 500-feat model
├─ 2000_Testing.ipynb              # eval notebook for 2000-feat model
├─ controller.ipynb                # utilities / shared logic
├─ gui_1.ipynb, gui_2.ipynb        # minimal GUI prototypes
├─ FAKE_CURRENCY_DETECTOR_REPORT.pdf  # full write-up
├─ pdf_project.pdf                 # additional doc
└─ README.md

📊 Approach (Short)

Preprocessing: resize/normalize note images; optional denoising.

Feature extraction: classical image descriptors (e.g., texture/edges/shape) aggregated to ~500 and ~2000-dimensional vectors.

Why two sizes? To compare accuracy vs. compute cost.

Modeling: train baseline ML models (e.g., SVM/LogReg/RandomForest).

Evaluation: accuracy, precision/recall, F1, confusion matrix; cross-validate and test on held-out set (see notebooks).

Demo: simple GUI notebooks to load an image and get a prediction.

The detailed method and screenshots are in FAKE_CURRENCY_DETECTOR_REPORT.pdf. 
GitHub
+1
