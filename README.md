# AICTE EDUNET Internship (Garbage Classification)
🧠 Goal:
    To classify images of garbage into different categories using a Convolutional Neural Network (CNN) enhanced by EfficientNetV2B2, a state-of-the-art pre-trained model.

📦 Steps Followed:

🔁 Imports & Libraries:
    Utilizes libraries like TensorFlow, Keras, Matplotlib, Seaborn, Scikit-learn, and Gradio.
    EfficientNetV2B2 is used for its efficiency and accuracy in image classification tasks.

📂 Data Handling:
    The dataset (Garbagedataset.zip) is uploaded and extracted.
    ImageDataGenerator is used for preprocessing and real-time data augmentation (e.g., rotation, zoom).

⚖️ Class Weights:
    compute_class_weight from sklearn is used to deal with class imbalance, improving model fairness and accuracy across classes.

🏗️ Model Architecture:
    Base model: 
      EfficientNetV2B2 (pre-trained on ImageNet, frozen initially).
    Custom top layers include:
      GlobalAveragePooling2D
      Dropout (regularization)
      Dense layers for classification

⚙️ Compilation & Training:
    Loss: categorical_crossentropy
    Optimizer: Adam
    Metrics: accuracy
    Callbacks: EarlyStopping (to avoid overfitting)
               ReduceLROnPlateau (to dynamically adjust learning rate)

📊 Evaluation:
    Accuracy and loss on validation set are measured.
    Detailed confusion matrix and classification report are generated to assess model performance per class.

🎯 Optional Fine-Tuning:
    After initial training, base model layers can be unfrozen for fine-tuning at a lower learning rate.

✅ Outcome:
   The model achieves reasonably high accuracy using transfer learning and handles class imbalance effectively.
   It is well-prepared for deployment in a user-facing application via Gradio.

