# Week 4 Quiz
## TOTAL POINTS 9

## Question 1
What does the acronym ETL stand for?
* External / Transform / Load
* Extract / Transfer / Load
* **Extract / Transform / Load**
* Enhance / Transfer / Load
> Correct

## Question 2
You have a multi processor machine, containing a CPU and GPU. How would you typically distribute these for training a model?
* Use CPU and GPU for all tasks in parallel
* Use CPU for extracting and the GPU for transforming and loading
* Use CPU for extracting and loading, and the GPU for transforming
* **Use CPU for extracting, transferring and loading, and the GPU for training**
> Correct

## Question 3
One way to speed up ETL is to use a cache. What’s the API for this called?
* tf.data.Dataset.ETLCache() 
* **tf.data.Dataset.cache()**
* tf.data.Dataset.datacache()
* tf.data.DataCache()
> Correct

## Question 4
I have a dataset loaded using this code: 
> dataset = tfds.load('cats_vs_dogs',split=tfds.Split.TRAIN)

How would I cache it on disk? 
* **train_dataset = dataset.cache(filename='cache')**
* train_dataset = dataset.cache(file='cache')
* train_dataset = dataset.cache(cachename=file)
* train_dataset = dataset.cache()
> Correct

Question 5
I have a dataset loaded using this code: 
> dataset = tfds.load('cats_vs_dogs',split=tfds.Split.TRAIN)

How would I cache it in memory?
* train_dataset = dataset.cache(cachename='memory')  
* train_dataset = dataset.memorycache()
* train_dataset = dataset.cache_in_memory()
* **train_dataset = dataset.cache()**
> Correct

## Question 6
If I create a function called ‘augment’ that transforms data, what code would I use to apply this after loading a dataset with 
> dataset = tfds.load('cats_vs_dogs',split=tfds.Split.TRAIN)
* augmented_dataset = dataset.augment()
* **augmented_dataset = dataset.map(augment)**
* augmented_dataset = dataset.augment(dataset)
* augmented_dataset = map(augment)
> Correct

## Question 7
If you want to parallelise the transform of a dataset across multiple cores, what’s the correct call?
* **s = dataset.map(augment, num_parallel_calls=2)**
* s = dataset.map(augment, 2)
* s = dataset.map(augment, parallel_calls=2)
* s = dataset.map(augment, num_parallel=2)
> Correct

## Question 8
If you’re not sure how many cores are accessible, for example, if you’re running in a shared cloud environment, how can you find out how many are available to you?
* num_cores = multiprocessing.available_cpus()
* It’s not possible
* **num_cores = multiprocessing.cpu_count()**
* num_cores = multiprocessing.cpu.count()
> Correct

## Question 9
The process of executing a custom map function over a batch of inputs is called:
* Batch mapping
* Map batching
* Visualization
* **Vectorization**
> Correct
