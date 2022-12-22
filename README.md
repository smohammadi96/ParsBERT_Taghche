# ParsBERT_Taghche

Sentiment Analysis

## dataset samples

![alt text](https://github.com/smohammadi96/ParsBERT_Taghche/blob/main/images/dataset_sample.png)

## Preprocessing
**1. remove extra columns**

**2. clean comments**
   - remove emojies
   - remove URLs
   - remove Hashtag
   - remove empty spaces
   - remove HTMLs
   - Normalization (Hazm)
  
 **3. classify rates**
 
   - rate >= 3 ==> 1
   - rate < 3 ==> 0

**4. balance dataset**

**Before:**

![alt text](https://github.com/smohammadi96/ParsBERT_Taghche/blob/main/images/chart1.png)

**After:**

![alt text](https://github.com/smohammadi96/ParsBERT_Taghche/blob/main/images/chart2.png)

## Results:

As you can see, the first graph shows the changes in the amount of loss in the two stages of train and validation during 10 epochs, which indicates that during the training process of the model there was too much fitted data and overfitting because The amount of loss has increased on the validation data, which means that the model has low generalizability. The second graph also shows the accuracy changes during 10 epochs in the train and validation stage.

![alt text](https://github.com/smohammadi96/ParsBERT_Taghche/blob/main/images/train_val_!.png)


![alt text](https://github.com/smohammadi96/ParsBERT_Taghche/blob/main/images/train_val_2.png)

By increasing the learning rate, the loss situation improved in the validation stage, but the accuracy of the model decreased drastically, and by adding augmentation and batch size, the accuracy improved and overfitting decreased.

![alt text](https://github.com/smohammadi96/ParsBERT_Taghche/blob/main/images/result.png)







