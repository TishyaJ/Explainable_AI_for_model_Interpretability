
🧠 Model Architecture
Model Type: Fully Connected Neural Network (Dense Sequential)

Input Shape: (4,) (4 features from the Iris dataset)

Layers:

Dense(64, activation='relu')

Dropout(0.2)

Dense(32, activation='relu')

Dropout(0.2)

Dense(3, activation='softmax') (for 3 iris classes)

Regularization: Dropout with rate 0.2 after each dense layer

Activation Functions:

Hidden layers: ReLU

Output layer: Softmax

🖼️ Visual Representation:

⚙️ Training Parameters
Optimizer: Adam

Loss Function: Sparse Categorical Crossentropy

Batch Size: 32

Epochs: 20

Learning Rate: Default (0.001), adaptive with ReduceLROnPlateau

Callbacks:

EarlyStopping (patience=5)

ReduceLROnPlateau (factor=0.5, min_lr=1e-6)

Validation Split: 20% of training data used for validation

📊 Dataset Details
Dataset Name: Iris dataset (from sklearn.datasets)

Number of Samples: 150

Number of Classes: 3 (Setosa, Versicolor, Virginica)

Class Distribution: 50 samples per class

Preprocessing:

Feature Scaling using StandardScaler

Optional: SMOTE available (not used here)

📈 Model Evaluation
Validation Accuracy: 76.7%

Validation Loss: 0.456

Confusion Matrix:

[[10  0  0]
 [ 0  4  6]
 [ 0  1  9]]


Classification Report:

Class	Precision	Recall	F1-score
0	      1.00	    1.00	 1.00
1	      0.80	    0.40	  0.53
2	      0.60	    0.90	  0.72

Overall Accuracy: 77%


