This project implements a Convolutional Neural Network (CNN) to classify images as either pizza or non-pizza. Using a dataset of images, the CNN achieves a test accuracy of 74%. Additionally, feature extraction from a fully connected layer of the CNN is utilized to train a Support Vector Machine (SVM) classifier for comparison, though the CNN outperforms the SVM in terms of accuracy, F1-score, and recall.
Model Architecture

The CNN model consists of:

    12 layers in total: 8 convolutional layers with pooling, and 4 fully connected layers.
    The final output layer uses a sigmoid activation function for binary classification.

Key performance metrics:

    Training Accuracy: ~74%
    Validation Accuracy: ~72%
    Test Accuracy: 74%

Data Preprocessing

Image data generators were employed to preprocess the dataset, ensuring robust learning and improved generalization. This included techniques such as image augmentation, rescaling, and normalization to enhance model performance.
Feature Extraction & SVM

After training the CNN, features were extracted from a fully connected layer with 400 units. These features were then used to train a linear and non-linear SVM:

    Non-Linear SVM (RBF Kernel): Achieved 56% accuracy.
    Linear SVM: Lower performance compared to the non-linear SVM.

The lower SVM accuracy suggests potential loss of information during feature extraction or limitations in capturing data complexity.
Conclusion

The CNN model demonstrated better performance with a test accuracy of 74%, outperforming the SVM model. The project highlights the strength of deep learning in image classification tasks, especially when compared to traditional machine learning models like SVM.
