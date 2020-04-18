## Classification with keras reuters dataset
classification with keras reuters dataset

### Train Data & Test Data
```
train_data    (8982)
train_labels  (8982)
test_data     (2246)
test_labels   (2246)
```
### Vectorizing and Normalizing
```
print("x_train ", x_train.shape)
print("x_test ", x_test.shape)
```

### One Hot encoding
```
print("one_hot_train_labels ", one_hot_train_labels.shape)
print("one_hot_test_labels ", one_hot_test_labels.shape)
```

### Model Summary
```
Model: "sequential_2"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
dense_4 (Dense)              (None, 256)               2560256   
_________________________________________________________________
dropout_3 (Dropout)          (None, 256)               0         
_________________________________________________________________
dense_5 (Dense)              (None, 256)               65792     
_________________________________________________________________
dropout_4 (Dropout)          (None, 256)               0         
_________________________________________________________________
dense_6 (Dense)              (None, 46)                11822     
=================================================================
Total params: 2,637,870
Trainable params: 2,637,870
Non-trainable params: 0
_________________________________________________________________
```

### Model Test
```
Test Loss and Accuracy
results  [3.1650060672760008, 0.6819999814033508]
dict_keys(['val_loss', 'val_accuracy', 'loss', 'accuracy'])
```
### Create Model with anonter data lable encoding structure
```
Model: "sequential_2"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
dense_6 (Dense)              (None, 64)                640064    
_________________________________________________________________
dense_7 (Dense)              (None, 64)                4160      
_________________________________________________________________
dense_8 (Dense)              (None, 46)                2990      
=================================================================
Total params: 647,214
Trainable params: 647,214
Non-trainable params: 0
_________________________________________________________________
```

### Model Training and The result (accuracy)
```
Epoch 1/10
16/16 [==============================] - 1s 45ms/step - loss: 3.2984 - acc: 0.3188 - val_loss: 2.6195 - val_acc: 0.3630
Epoch 2/10
16/16 [==============================] - 1s 40ms/step - loss: 2.0683 - acc: 0.5480 - val_loss: 1.6871 - val_acc: 0.6340
Epoch 3/10
16/16 [==============================] - 1s 64ms/step - loss: 1.3894 - acc: 0.7003 - val_loss: 1.2945 - val_acc: 0.7000
Epoch 4/10
16/16 [==============================] - 1s 68ms/step - loss: 1.0593 - acc: 0.7657 - val_loss: 1.1253 - val_acc: 0.7610
Epoch 5/10
16/16 [==============================] - 1s 68ms/step - loss: 0.8358 - acc: 0.8250 - val_loss: 1.0233 - val_acc: 0.7830
Epoch 6/10
16/16 [==============================] - 1s 68ms/step - loss: 0.6585 - acc: 0.8623 - val_loss: 0.9483 - val_acc: 0.8030
Epoch 7/10
16/16 [==============================] - 1s 68ms/step - loss: 0.5114 - acc: 0.8935 - val_loss: 0.9038 - val_acc: 0.8110
Epoch 8/10
16/16 [==============================] - 1s 65ms/step - loss: 0.4010 - acc: 0.9181 - val_loss: 0.8900 - val_acc: 0.8180
Epoch 9/10
16/16 [==============================] - 1s 40ms/step - loss: 0.3196 - acc: 0.9326 - val_loss: 0.8763 - val_acc: 0.8210
Epoch 10/10
16/16 [==============================] - 1s 41ms/step - loss: 0.2566 - acc: 0.9440 - val_loss: 0.8923 - val_acc: 0.8160
```
