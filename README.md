# Medical-imaging
Brain Tumor Detection & Localization (CNN + ResUNet)

This project applies deep learning models to detect the presence of brain tumors from MRI scans (classification) and localize the tumor regions (segmentation). It uses a CNN classifier for binary tumor detection and a ResUNet segmentation model for tumor localization.

Includes:

Classifier (CNN): Detects whether a tumor exists in an MRI scan.

Segmentation (ResUNet): Localizes tumor region with pixel-level accuracy.

Visualization: Outputs segmentation masks overlayed on MRI images.

 Setup

Clone the repo git clone https://github.com/your-username/brain-tumor-ai.git cd brain-tumor-ai

Create & activate virtual environment python3 -m venv .venv source .venv/bin/activate # Linux/Mac .venv\Scripts\activate # Windows

Install dependencies pip install -r requirements.txt

 Usage

Train Tumor Classifier python train_classifier.py

Train ResUNet Segmentation Model python train_resunet.py

Evaluate Model python evaluate.py --model resunet --images /path/to/test/images

Run Visualization (Sample) python visualize.py --image sample_mri.png

 Future Work

Extend to 3D MRI volumes.

Experiment with transformer-based segmentation (e.g., Swin-UNet, nnUNet).

Deploy as a Streamlit web app for radiologists.
