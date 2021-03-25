# Week 2 Quiz
## Latest Submission Grade: 100%

# Question 1
How do you use Image Augmentation in TensorFLow?
* You have to write a plugin to extend tf.layers
* **Using parameters to the ImageDataGenerator**
* With the keras.augment API
* With the tf.augment API
> Correct

# Question 2
If my training data only has people facing left, but I want to classify people facing right, how would I avoid overfitting?
* Use the ‘flip_vertical’ parameter around the Y axis
* **Use the ‘horizontal_flip’ parameter**
* Use the ‘flip’ parameter
* Use the ‘flip’ parameter and set ‘horizontal’
> Correct

# Question 3
When training with augmentation, you noticed that the training is a little slower. Why?
* **Because the image processing takes cycles**
* Because the augmented data is bigger
* Because there is more data to train on
* Because the training is making more mistakes
> Correct

Question 4
What does the fill_mode parameter do?
* There is no fill_mode parameter
* It creates random noise in the image
* **It attempts to recreate lost information after a transformation like a shear**
* It masks the background of an image
> Correct

Question 5
When using Image Augmentation with the ImageDataGenerator, what happens to your raw image data on-disk.
* It gets overwritten, so be sure to make a backup
* A copy is made and the augmentation is done on the copy
* **Nothing, all augmentation is done in-memory**
* It gets deleted
> Correct

Question 6
How does Image Augmentation help solve overfitting?
* It slows down the training process
* **It manipulates the training set to generate more scenarios for features in the images**
* It manipulates the validation set to generate more scenarios for features in the images
* It automatically fits features to images by finding them through image processing techniques
> Correct

Question 7
When using Image Augmentation my training gets...
* **Slower**
* Faster
* Stays the Same
* Much Faster
> Correct

Question 8
Using Image Augmentation effectively simulates having a larger data set for training.
* False
* **True**
> Correct
