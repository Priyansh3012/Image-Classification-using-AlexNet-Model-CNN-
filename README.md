# Image-Classification-using-AlexNet-Model-CNN-

This project demonstrates the construction and optimization of an image classification model using AlexNet. Through systematic hyperparameter tuning and careful analysis of training dynamics, overfitting was mitigated, resulting in a model that performs well on both training and unseen data. Despite the limited dataset, the model achieved a reasonable validation accuracy and correctly predicted new images, showcasing the robustness and potential of CNNs in image classification tasks. Future work could involve expanding the dataset and exploring additional regularization techniques to further enhance model performance.

## Tools and Libraries Used:
1. Python (programming language)
2. Pandas
3. Numpy
4. Matplotlib
5. OpenCV (for image processing)
6. TensorFlow and Keras (for building and training the model)
7. Keras Tuner (for hyperparameter tuning)
 
## Techniques:
 * Label Encoding
 * One-Hot Encoding
    
## Key Steps and Methodology:

 * Data Preparation:
 * Images were labeled and encoded using label encoding followed by one-hot encoding.
 * OpenCV was used to read and preprocess the images.
   
## Model Building:

* An initial **AlexNet model(CNN)** is build.
* **Keras Random Search tuner** was utilized to perform hyperparameter tuning.

## Hyperparameter Tuning Results:

Optimal parameters identified:

* **First convolutional layer:** 128 filters, kernel size 5
* **Second convolutional layer:** 64 filters, kernel size 3
* **Third convolutional layer:** kernel size 3
* **Dense units:** 256
* **Learning rate:** 0.0001
  
## Training and Evaluation:

 * The model was retrained using the tuned parameters.
 * The model was trained for 30 epochs initially.
 * Plotted model accuracy and loss graphs for both training and validation data.

## Overfitting Analysis:

* Noticed overfitting as the validation loss increased after **17 epochs**.
* **Retrained the model for 17 epochs to mitigate overfitting.**
* Achieved a validation accuracy of **61.9%**.

  ![image](https://github.com/user-attachments/assets/eb7ced20-74b8-4e91-b05e-e856e308148b) ![image](https://github.com/user-attachments/assets/802b6800-6331-4003-940a-328ab2fde8db)



## Prediction:

* The final model was tested on new unseen images and correctly predicted the classes.

  ![image](https://github.com/user-attachments/assets/a89c14ee-6353-43f1-878c-f1353fd04c5b)

## Key Findings and Analysis:

* **Hyperparameter Tuning:** Optimal hyperparameters significantly improved the model's performance.
* **Overfitting:** Initial training revealed overfitting after 17 epochs, which was corrected by reducing the number of epochs.
* **Model Performance:** The final model, after tuning and addressing overfitting, achieved a validation accuracy of 61%, which was constrained by the limited dataset size.

## Conclusion:

* This project successfully demonstrated the construction and optimization of an image classification model using AlexNet. By systematically tuning hyperparameters and addressing overfitting, the model achieved a validation accuracy of 61.9% despite the limited dataset size. The final model accurately predicted new, unseen images, showcasing its effectiveness. Future improvements could include expanding the dataset and exploring additional regularization techniques to further enhance performance. This project highlights the power and potential of CNNs in image classification tasks, providing a solid foundation for more advanced applications.

