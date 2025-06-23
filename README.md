# 🤖 Rock-Paper-Scissors Image Classification

Train a lightweight CNN to distinguish rock, paper, and scissors hand poses using 300×300 images.

---

## 🗂️ Project Layout

/
├── data/ # 300×300 images (train/, valid/, test/)
└── code/ # Training scripts & notebooks


---

## 🚀 Quickstart

1. **Clone**  
   ```bash
   git clone https://github.com/<your-username>/rock-paper-scissors-classification.git
   cd rock-paper-scissors-classification

2. **Install dependencies**

   pip install tensorflow matplotlib numpy

3. **Train**

   python code/train_rps.py --data_dir data/rock-paper-scissors

4. **Evaluate & visualize**

   Saved model: models/rps_cnn.h5

  Loss curve: figures/loss_curve.png

  Confusion matrix: figures/confusion_matrix.png



🔍 **Highlights**

  Data Preprocessing: Rescale to [0,1], augment (flip, rotate) on 300×300 inputs

  Architecture: 2×Conv(3×3)+Pool → Flatten → Dense(128) → Softmax(3)

  Training: Adam optimizer, categorical crossentropy, 10 epochs, batch size 32

  Performance: ~96% test accuracy


👤 **Author**

  Farzaneh Yousefi


