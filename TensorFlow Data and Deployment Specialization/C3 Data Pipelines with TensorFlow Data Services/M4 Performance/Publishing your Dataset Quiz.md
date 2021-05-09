# Publishing your Dataset Quiz
## TOTAL POINTS 8

## Question 1
If you want to create your own dataset and add it to TFDS, what class do you need to override?
* DataBuilder
* DatasetBuild
* **DatasetBuilder**
* Dataset
> Correct

## Question 2
If you want your dataset to have splits such as TRAIN or VALIDATION what class do you need to use?
* FileSplitter
* **FileAdapterBuilder**
* FileSplitBuilder
* SplitBuilder
> Correct

## Question 3
What class allows you to create your own dataset, add it to TFDS, define splits, and have it generate examples from source data?
* There is no single class, you have to use multiple APIs 
* DatasetBuilder
* FileAdapterBuilder
* **GeneratorBasedBuilder**
> Correct

## Question 4
What Python script in TFDS gets you started with creating a new dataset?
* **create_new_dataset.py**
* new_dataset.py
* create_new_tfds_dataset.py
* create_dataset.py
> Correct

## Question 5
When creating a dataset using GeneratorBasedBuilder, what three methods do you need to implement?
* **_info(), _split_generators(), _generate_examples()**
* _info(), _split_generators(), _examples_generators()
* _info(), _split(), examples()
* _info(), _generate_splits(), _generate_examples()
> Correct

## Question 6
Your dataset will need to download data from the web or cloud to your user’s machine. What class in TFDS must the download and extract process go through?
* tfds.download.Manager
* **tfds.download.DownloadManager**
* tfds.DownloadManager
* tfds.manager.Download
> Correct

## Question 7
If your dataset requires extra dependencies that aren’t part of TFDS or TensorFlow, and your user doesn’t have them, how do you ensure they get installed?
* Add imports for the required dependencies to your setup.py
* Define them in DATASET_EXTRAS as lazy loads for all datasets
* Lazy load them in your setup.py
* **Define them in DATASET_EXTRAS as lazy loads just for your dataset**
> Correct

## Question 8
Where do you store citations for your dataset?
* DatasetInfo.bibtexcitation
* DatasetInfo.citations
* DatasetInfo.bibtex
* **DatasetInfo.citation**
> Correct
