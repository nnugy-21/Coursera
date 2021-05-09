# Week 3 Quiz
## TOTAL POINTS 8

## Question 1
What is the name of the tf.data class that represents a sequence of elements, in which each item consists of one or more components?
* tf.data.data.Set
* tf.data.Sequence
* tf.dataset.Data
* **tf.data.Dataset**
> Correct

## Question 2
Which of these are types of feature column (choose 2)?
* Integer Column
* Data Column
* **Categorical Column**
> Correct
* **Dense Column**
> Correct

## Question 3
If you want to map a person’s birth year to a decade, what’s the best column type to use?
* DecadeColumn
* **BucketizedColumn**
* StringColumn
* YearColumn
> Correct

## Question 4
You have a list of vocabulary words, and you want to one-hot encode them to a column. What’s the appropriate type?
* tf.feature_column.categorical_column_with_vocab  
* **tf.feature_column.categorical_column_with_vocabulary_list**
* tf.feature_column.categorical_column_with_list  
* Tf.feature_column.categorical_column_with_list_vocabulary
> Correct

## Question 5
How do you turn a Numpy array into a Dataset?
* **Using from_tensor_slices**
* Using from_numpy_array
* Using load_numpy
* Using load_tensors_from_numpy
> Correct

## Question 6
When using pandas, how do you automatically one-hot encode a column?
* Using pd.Encode.Category
* Using pd.OneHot
* **Using pd.Categorical**
* Using pd.Category
> Correct

## Question 7
What experimental API allows you to quickly turn a CSV into a dataset?
* tf.data.experimental.make_dataset
* tf.data.experimental.make_csv
* tf.data.experimental.csv_dataset
* **tf.data.experimental.make_csv_dataset**
> Correct

## Question 8
What API is used to load text from a file into a dataset?
* tf.data.LineDataset
* tf.dataset.TextDataset
* tf.data.TextDataset
* **tf.data.TextLineDataset**
> Correct
