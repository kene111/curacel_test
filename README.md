# curacel_test


### Repository Breakdown:
1) toyota-model-recognition-service-0: The .ipynb notebook contains the code that handles preprocesses, trains, and test the models performance. This model trains on the dataset regardless of the imabalance.
2) toyota-model-recognition-service-1: This .ipynb notebook code tries to correct the imabalanced image dataset.
3) Dataset Origin:  https://www.kaggle.com/occultainsights/toyota-cars-over-20k-labeled-images
4) Dataset Used: https://www.dropbox.com/s/8hq66n5xv264xsm/car_image_data.zip?dl=0
5) Models: https://drive.google.com/drive/folders/1lx0ZbDserY9g4FOhndS6f5Tv9H9L0tvW?usp=sharing


Model Performance:
1)  toyota_model_0.h5 (corresponding to toyota-model-recognition-service-0 notebook) :
- validation_loss: 5.3786
- validation_accuracy: 0.02048
- training_accuracy: 0.6421
- training_loss:1.1620

Model performance was very poor.

2)  toyota_model_1.h5 (corresponding to toyota-model-recognition-service-1 notebook) :
- validation_loss: 3.6997
- validation_accuracy: 0.0628
- training_accuracy: 0.9917
- training_loss: 0.3181

Even with the use of the keras-balanced-batch-generator the validation accuracy was still poor, yet this model performed better than the first model.


##### This also shows that the models over-fitted.

### Note:
1) The dataset is imbalanced. In order to curb the imbalanced image data ( The maximum number of images per model used was 350, while the minimum  number of images per model used was 22 i.e some toyota models only had 22 images)
2) Notebook was trained on kaggle due to how large the dataset is. 
3) Model could not be uploaded to github due to how large it is.


### Other possible solutions to solving the imbalanced dataset:
1) dropping the toyota models with cars lower than 100 images.
2) Using GANs to generate more image data for the lower classes.

#### Models overall performance could be improved if given more time for hyperparameter tuning.



