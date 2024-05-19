# Task4-Hand-Gestures

Dataset :-  https://www.kaggle.com/gti-upm/leapgestrecog

## **MODEL**
1. **Modular Model Building:**
   - We want to make our model organized and easy to understand, so we create two building blocks: a convolution block and a dense layer block.
   - Convolutional Neural Network (CNN) is used for image-related tasks, and these blocks help structure the CNN.

2. **Model Architecture:**
   - The model will be designed to detect pneumonia in X-ray images.
   - Dropout layers are used to prevent the model from becoming too specialized on the training data, reducing the chance of overfitting.

3. **Output Layer:**
   - The model's final layer is a Dense layer with one node.
   - Since we have only two possible labels (pneumonia or not pneumonia), a single node is sufficient for binary classification.

4. **Loss Function:**
   - Binary Crossentropy is chosen as the loss function.
   - It measures the difference between the predicted probabilities and the true labels for binary classification tasks.

5. **Class Weights:**
   - Class weights are considered during training.
   - They help address the imbalance in the dataset, as there may be more examples of one class than the other.

6. **Metrics:**
   - Precision and Recall are chosen as evaluation metrics.
   - Accuracy can be misleading when classes are imbalanced, so precision and recall provide a more detailed understanding.
   - Precision: Proportion of correctly predicted positive cases out of all predicted positive cases.
   - Recall: Proportion of correctly predicted positive cases out of all actual positive cases.

7. **Training on TPU:**
   - Training on a Tensor Processing Unit (TPU) can speed up the training process.
