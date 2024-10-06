### Vehicle Recognition with MobileNet:
This project involves vehicle type recognition from images using the **MobileNet** model. Here’s an overview of the process and key details:

#### 1. **Libraries Used:**
   - Various libraries such as **TensorFlow**, **Keras**, **OpenCV**, and **NumPy** were used for data preparation, model building, and image processing.

#### 2. **Data Preparation:**
   - A directory of images with four different vehicle categories (`Bus`, `Car`, `Truck`, `Motorcycle`) is loaded.
   - Images are read with OpenCV and resized to a standard size of 224x224 pixels.
   - The images and labels are then stored in lists and shuffled randomly into arrays `x` and `y`.
   - #### Sample of DataSet:
![Image_14](https://github.com/user-attachments/assets/8ce1612a-2767-462d-ade9-d3c0d9d6b09b)
![Image_21](https://github.com/user-attachments/assets/2e9c512d-2179-45d5-8956-827b4f7444a7)
![Image_17](https://github.com/user-attachments/assets/36d02d65-f3ff-4246-a8ff-6e2a9b1b33d9)
![Image_16](https://github.com/user-attachments/assets/799fda16-238a-4729-8b6c-bcceca7c26a2)

#### 3. **Label Encoding and Data Splitting:**
   - Labels are converted to **One-Hot Encoded** format.
   - The data is split into **training** (80%) and **testing** (20%) sets.

#### 4. **Data Augmentation:**
   - Data augmentation techniques like rescaling, rotation, shifting, and flipping are applied to improve model performance and prevent overfitting.

#### 5. **MobileNet Model:**
   - A pre-trained **MobileNet** model is used for feature extraction, with its layers set as non-trainable.
   - A **Flatten** layer and a **Dense** layer with a **Softmax** activation function are added for final classification.

#### 6. **Training Setup:**
   - The model is compiled using the **Adam** optimizer and **Categorical Crossentropy** as the loss function.
   - **ModelCheckpoint** and **EarlyStopping** callbacks are employed to save the best weights and prevent overfitting.

#### 7. **Model Training and Validation:**
   - The model is trained over 5 epochs, with accuracy metrics calculated on the validation data.
   - Accuracy :
     
   ![Screenshot 2024-10-06 190030](https://github.com/user-attachments/assets/9b8da493-c66b-4866-8e5a-2fd6cfac9f70)


### Conclusion:
This project builds a vehicle recognition system using MobileNet, which can classify vehicle types into four categories. Data processing, modeling, and training setups are optimized, leveraging common methods to enhance accuracy and efficiency.
