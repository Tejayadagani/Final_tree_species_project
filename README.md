# Final_tree_species_project
Tree Species Image Classification Project
This project involves classifying images of tree species using deep learning. It evaluates and compares three different CNN-based models:

✅ Basic CNN

✅ CNN with Batch Normalization

✅ Transfer Learning using EfficientNetB0

Each model is trained on the same dataset and evaluated based on validation accuracy and loss.

📁 Dataset
Dataset source: Kaggle Tree Species Dataset

Structure:

Copy
Edit
dataset/
  ├── class_1/
  │     ├── image1.jpg
  │     ├── image2.jpg
  ├── class_2/
  │     ├── image1.jpg
  │     ├── image2.jpg
  ...
🧠 Models Implemented
Model	Description	Output File
Basic CNN	Simple architecture with Conv2D + Dense layers	basic_cnn_model.h5
CNN + Batch Normalization	Adds batch normalization after conv layers	cnn_batchnorm_model.h5
EfficientNetB0 (Transfer)	Uses pretrained EfficientNet base	efficientnet_model.h5

📦 Dependencies
Install via pip if needed:

bash
Copy
Edit
pip install tensorflow matplotlib numpy
🔧 Training Setup
All models are trained using the same settings:

Image size: 224x224

Batch size: 32

Epochs: 10

Optimizer: Adam (lr = 0.001)

Loss: Categorical Crossentropy

Data Augmentation: Rotation, shift, shear, zoom, flip

📊 Results
Each model produces a training and validation accuracy/loss plot for analysis.

Example output:

Model Accuracy

Basic CNN: ~85%

CNN + BN: ~88%

EfficientNetB0: ~93%

🧪 How to Run
In Google Colab or Jupyter Notebook:

python
Copy
Edit
# Mount Drive (if needed)
from google.colab import drive
drive.mount('/content/drive')

# Run preprocessing, training, and evaluation code (see .ipynb)
After training, you will see validation accuracy/loss graphs for each model.

📁 Output Files
The following models are saved:

basic_cnn_model.h5

cnn_batchnorm_model.h5

efficientnet_model.h5

These files can be used for inference, app deployment, or further fine-tuning.

📈 Evaluation Graphs
Training history is visualized using matplotlib for all three models.

Train vs Val Accuracy

Train vs Val Loss

🔮 Future Improvements
Hyperparameter tuning

Fine-tuning pretrained EfficientNet

Add test set evaluation

Deploy via Flask/Streamlit

🤝 Authors & Credits
Developed by Dharma Yadagani

Dataset by Vidit Gandhi on Kaggle
