# curacel_test


### Repository Breakdown:
1) toyota-model-recognition-service-0: The .ipynb code that handles preprocesses, trains, and test the model. This model trains on the dataset regardless of the imabalance.
2) toyota-model-recognition-service-1: This .ipynb code tries to correct the imabalanced data.
3) Dataset:  https://www.kaggle.com/occultainsights/toyota-cars-over-20k-labeled-images
4) Model: https://drive.google.com/drive/folders/1lx0ZbDserY9g4FOhndS6f5Tv9H9L0tvW?usp=sharing


### 


Model Performance:
1)  toyota_model_0.h5 (corresponding to toyota-model-recognition-service-0 notebook) :
- validation_loss: 5.3786
- validation_accuracy: 0.02048
- training_accuracy: 0.6421
- training_loss:1.1620

##### This shows that the model over-fitted

### Note:
1) The dataset is imbalanced.
2) Notebook was trained on kaggle due to how large the dataset is. 
3) Model cannot be uploaded to gitbuh due to how large it is.



