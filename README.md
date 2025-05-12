# 🛒 Good Seed Age Verification Model

## 📌 Project Description
This project supports the Good Seed supermarket chain in complying with alcohol laws by ensuring that alcohol is not sold to underage individuals. To achieve this, I developed and evaluated a deep learning regression model capable of predicting a customer's age using facial images captured at checkout counters.

The task involved training a computer vision model on a labeled dataset of photographs, where each image corresponds to an individual’s actual age. The model’s objective was to estimate age with high accuracy—particularly distinguishing whether individuals are legally permitted to buy alcohol.

## 📊 Table of Contents
  - Project Description
  - Tools and Libraries Used
  - How to Run
  - Model Training and Evaluation
  - Conclusion
  - Credits
  - License

## ⚙️ Tools and Libraries Use
  - Python 3.10+
  - TensorFlow / Keras
  - Pandas, NumPy
  - Matplotlib
  - Jupyter Notebook
  - GPU-enabled computing platform (for model training)

## 🧪 How to Install and Run
  1. Clone the repository:
     ```bash
     git clone https://github.com/your-username/good-seed-age-verification.git
     cd good-seed-age-verification
  3. Install dependencies:
     ```bash
     pip install -r requirements.txt
  4. Run the notebook on a GPU-supported platform (e.g., Google Colab, Kaggle, or a local CUDA-enabled environment):
     ```bash
     notebook.ipynb

##🧠 Model Training and Evaluation
The model was trained for 20 epochs using a CNN-based architecture. Key performance metrics included:
  - Training Loss (MSE): Decreased steadily from 95.35 to 17.03
  - Training MAE: Dropped from 7.43 to 3.18, indicating effective learning
  - Validation MAE: Best at epoch 17 (6.64), minimal improvement after epoch 10
  - Validation Loss: Fluctuated, spiked at epoch 12 (185.63), lowest at epoch 17 (78.43)

### Signs of Overfitting Detected:
  - Training loss continued to decline while validation error plateaued after epoch 8
  - Validation MAE showed little improvement beyond epoch 10

### Best Model Epoch: Epoch 17 — lowest validation MAE and balanced performance

## ✅ Conclusion
The age prediction model for Good Seed shows promising results in estimating customer age from facial images, helping the chain comply with legal alcohol sale requirements. Though the model fits training data well, overfitting signs on the validation set suggest further improvements could include:
  - Data augmentation to generalize better
  - Regularization techniques
  - Early stopping to prevent performance decay
Despite these, the model demonstrates practical usability, with the best performance achieved at epoch 17.

## 🤝 Credits
This project was created as part of the TripleTen Data Science program. Special thanks to:
  - TripleTen instructors and peers for ongoing support and feedback.
  - Facial image dataset provided as part of the project materials.

## 🛡️ License
This project is licensed under the MIT License.

