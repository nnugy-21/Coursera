# Week 2
## TOTAL POINTS 7

## Question 1
If you want to merge two splits 'train' and 'test' together using Splits API, how would you be able to do so?
* tfds.load('mnist',split = np.concat('train+test'))
* tfds.load('mnist', merge = 'train+test')
* tfds.load('mnist', split = pd.concat('train', 'test'))
* **tfds.load('mnist', split = 'train + test')**
> Correct<br>
Correct!<br>
Passing both train and test in the string is the proper way to get both the splits.

## Question 2
The MNISTv3 dataset supports the Splits API. The train split has 70000 records in it. If you just want to create a subsplit of the first 7000 records and want to use the python slicing notation instead of Splits API, what would be the answer?
* tfds.load('mnist:3.*.*', subsplit='train[:7000]')
* tfds.load('mnist:3.*.*', split='train[7000:]')
* **tfds.load('mnist:3.*.*', split='train[:7000]')**
* Read the entire train split, create a new dataset, iterate over the first 7000 of the 70000, and copy the records one-by-one to the new dataset.
> Correct<br>
Correct!<br>
train[:7000] technically takes records from 0 to 6999 index value.

## Question 3
If you want a subsplit of the first 10% of the MNISTv3 training records, what would the code look like using the Splits API?  
* tfds.load('mnist:3.*.*', subsplit='test[10%:]') 
* **tfds.load('mnist:3.*.*', split='test[:10%]')**
* tfds.load('mnist:3.*.*', subsplit='test[:10%]')
* tfds.load('mnist:3.*.*', split='test[10%:]')
> Correct<br>
Correct!<br>
'test[:10%]' in string format represents that we want the first 10% of the records from the test split.

## Question 4
How many validation splits will this code generate?
> val_ds = tfds.load('mnist:3.*.*', split = ['train[{}]%:{}%]'.format(k/4,(k+40)/4) for k in range(0,400,40)])
* 5
* 40
* **10**
* Will throw an Error
> Correct<br>
Correct!<br>
As k is incrementing by 40, you get the values like (0,40), (40,80)... until the last one, (360:400).<br>
Dividing each value by 4 as you have (k/4,(k+40)/4), it will get converted to [0,10],[10,20]...[90,100] which is 10 splits.

## Question 5
True or False : The TFRecord shards are only created for the training data.
* **False**
* True
> Correct<br>
If your validation and test data size is bigger, they also can get sharded.

## Question 6
Which of the following could be used to investigate how the TFRecords files look like?  
> filename = "your_tf_record_file"<br>
raw_file = tf.keras.dataset.load(filename)<br>
for raw_record in raw_file.take(1):<br>
print(repr(raw_record))

> **filename = "your_tf_record_file"<br>
raw_file = tf.data.TFRecordDataset(filename)<br>
for raw_record in raw_file.take(1):<br>
print(repr(raw_record))**

> filename = "your_tf_record_file"<br>
raw_file = tf.loads(filename)<br>
for raw_record in raw_file.take(1):<br>
    print(repr(raw_record))

> filename = "your_tf_record_file"<br>
raw_file = tf.RecordDataset(filename)<br>
for raw_record in raw_file.take(1):<br>
    print(repr(raw_record))
> Correct<br>
Correct!<br>
tf.data.TFRecordDataset is used to read your raw TFRecord files and convert it to an object.<br>
take(1) gives you 1 record from the raw_file TFRecordDataset object.<br>
repr() function returns a printable representation of the given tfrecord object.


## Question 7
Below is an example of how raw TFRecord files look like when you properly read and print them with TFRecordDataset methods. 
![image](https://user-images.githubusercontent.com/79896959/117546204-75334300-b053-11eb-84a2-389fecbb9ace.png)


To parse them into proper format, which of the following options need to be implemented?

* Apply the parsing function to each item in the dataset using the keras.dataset.map method
* **Apply the parsing function to each item in the dataset using the tf.data.Dataset.map method.**
> Correct<br>
Correct!<br>
This is Step 3. You need ot parse each file individually and map them to the parsing function to create clean, readable standard tensors.
* Creating a parsing function using tfds.load()
* **Creating a feature description dictionary**
> Correct<br>
Correct!<br>
This is Step 1. You need to define your feature descriptions properly based on the dataset and its metadata.This is necessary here because datasets use graph-execution, and need description to build their shape and type signature<br>
* **Creating a parsing function using tf.io.parse_single_example()**
> Correct<br>
Correct!<br>
This is Step 2. tf.io.parse_single_example() is used to parse examples one by one as the raw TFRecordDataset files contain serialized tf.train.Example objects.<br>
You can also use tf.parse_exampleto parse the whole batch at once.
