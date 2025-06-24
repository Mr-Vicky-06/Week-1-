# AICTE EDUNET Internship (Garbage Classification)

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

