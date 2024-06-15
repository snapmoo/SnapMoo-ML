<div align="center">
  <h1>Machine Learning</h1>
  <img src="https://raw.githubusercontent.com/snapmoo/snapmoo/main/assets/Machine%20Learning/TensorFlow.png" alt="TensorFlow" width="40%">
</div>
<br>
<div>
  <h2>Overview</h2>
  <p>
    Machine Learning is tasked with processing the dataset and building a model that will be used to process images of cow limbs that will be detected to determine whether the cow is infected with FMD or not. 
  </p>
</div>
<br>
<div>
  <h2>Dataset</h2>
  <p>
    The dataset used to build the model is a dataset containing images of healthy cattle parts and FMD-infected cattle parts. 
    <a href="https://zenodo.org/records/7779246">FMD_Cattle</a>
  </p>
</div>
<br>
<div>
  <h2>Model Architecture</h2>
  <p>
  The trained model is a Convolutional Neural Network (CNN) architecture model using TensorFlow. In this application, we created a model by using transfer learning from the VGG16 base model in building the model and using the 'FMD Cattle' dataset which has been divided into 3 data groups, namely 70% train data, 15% validation data, and 15% test data. The model accuracy result obtained is 0.9553 with validation accuracy of 0.9688 after we use a callback to stop the train model after the accuracy and validation accuracy are above 0.95 and show an ideal model plot. As for after prediction on test data, the output is obtained that the model successfully predicts all test data correctly and accurately.
    <details>
      <summary>Model Summary</summary>
      <img src="https://raw.github.com/snapmoo/snapmoo/main/assets/Machine%20Learning/Model%20Summary.jpg" alt="Model Summary" class="dropdown-image">
    </details>
    <details>
      <summary>Accuraccy & Loss</summary>
      <img src="https://raw.github.com/snapmoo/snapmoo/main/assets/Machine%20Learning/Accuracy.jpg" alt="Accuracy Model" class="dropdown-image">
      <img src="https://raw.github.com/snapmoo/snapmoo/main/assets/Machine%20Learning/Loss.jpg" alt="Loss Model" class="dropdown-image">
    </details>
  </p>
</div>
<div>
  <h2>Tolls</h2>
  <p>
    - Google Colab serves as a platform to execute Python programming syntax such as data preprocessing, model building, and model evaluation.
  </p>
</div>
<div>
  <h2>Timeline</h2>
    <h4>Stage 1: Gathering and Cleaning Dataset</h4>
      <p>
        Gathering the dataset and cleaning the dataset where we removed inappropriate images and added some images from Google. Then, the processed dataset was uploaded to the ML team's Goggle Drive so that it could be accessed by all members.
      </p>
    <h4>Stage 2: Image Preprocessing and Data Augmentation</h4>
      <p>
        We perform various types of preprocessing on the datasets to try each type of dataset to avoid overfitting or underfitting and to improve model curation. Some types of datasets are:
        <br>1. The original dataset is without the addition of images from Google and without augmentation. 
        <br>2. Datasets that have added several images from Google and without augmentation.
        <br>3. Original dataset that is without the addition of images from Google and has been augmented. 
        <br>4. Dataset that has been added several images from Google and has been augmented.
      </p>
    <h4>Stage 3: Build The Model</h4>
      <p>
        Build the model architecture using TensorFlow. Try various CNN model architectures ranging from training from scratch (without using transfer learning) to using transfer learning from the VGG16 base model.
      </p>
    <h4>Stage 4: Convert to TFLite and Ready For Deployment</h4>
      <p>
      Convert the model to TFLite using tensorflow
      </p>
    <h4>Stage 5: Optimizing Model Performance</h4>
      <p>
      Improve the performance of the model when the accuracy results are still not good continuously until finding the best model and can be used in applications with the best accuracy.
      </p>
    <h4>Stage 6:  Repeating the above process </h4>
      <p>
      When the model obtained is not good enough, it will return to stage 2 and so on to select datasets that have been augmented or not, in an effort to improve the accuracy of the model. Until now, we have found a model with the best accuracy and can predict the testing data well.
      </p>
</div>

