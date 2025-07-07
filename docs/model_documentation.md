
🧠 Model Architecture
Model Type: Fully Connected Neural Network (Dense Sequential)

Input Shape: (4,) (4 features from the Iris dataset)

Layers:
- Dense(64, activation='relu')
- Dropout(0.2)
- Dense(32, activation='relu')
- Dropout(0.2)
- Dense(3, activation='softmax') (for 3 iris classes)

Regularization: Dropout with rate 0.2 after each dense layer

Activation Functions:
- Hidden layers: ReLU
- Output layer: Softmax

🖼️ Visual Representation:
- model_architecture.png

⚙️ Training Parameters
- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy
- Batch Size: 32
- Epochs: 20
- Learning Rate: 0.001 (adaptive with ReduceLROnPlateau)
- Callbacks: EarlyStopping (patience=5), ReduceLROnPlateau
- Validation Split: 20%

📊 Dataset Details
- Dataset: Iris dataset (from sklearn.datasets)
- Samples: 150
- Classes: 3 (Setosa, Versicolor, Virginica)
- Preprocessing: StandardScaler

📈 Model Evaluation
- Validation Accuracy: 76.7%
- Validation Loss: 0.456

Confusion Matrix:
[[10  0  0]
 [ 0  4  6]
 [ 0  1  9]]

Classification Report:
Class    Precision  Recall  F1-score
0        1.00       1.00    1.00
1        0.80       0.40    0.53
2        0.60       0.90    0.72

Overall Accuracy: 77%
