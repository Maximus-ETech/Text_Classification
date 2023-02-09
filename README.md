This project “Text_classification” solves multi-class text classification tasks ,i.e any piece of text(documents/forms/IT tickets/Emails) can be tagged/classified with a set of pre-defined categories.
The notebooks are designed in more generic way that any user can run these with their text data to classify into pred-defined categories by following some basic steps:
For now, the notebooks can be run with data in “CSV”  and “folder”format.
If the data is in CSV format then the steps to be followed are:
1.	Download the repository.
2.	The input text column which is the main feature that goes into the model should be named “Content” and the target variable should be named as “Label” (This step should be followed in order to run the notebooks without any user interference)
3.	Set your current working directory in .env file. It has 3 paths,
a)	csv_input_dir– put the path where the training data is saved , the name of the data file should be “train_data”
b)	output_model_dir – put the path where you wanted to store the output(it can be model, evaluation results, prediction results)
c)	test_input_dir- put the path where the inference data is saved, the name of the data file should be “test_data”
4.	Run the requirements.txt file and download the libraries.
5.	Run the notebook ‘’text_classification_training” and the output is the model that has been trained on the data(Content) and labels(Label).
6.	Run the notebook “text_classification_inference”  to find the labels fo the test data(Content). The results are stored in csv file and are saved in the output folder.
If the data is in File fomat hierarchy like below:
├── datadir
    │   ├── train
    │   │   ├── class0       # folder containing documents of class 0
    │   │   ├── class1       # folder containing documents of class 1
    │   │   ├── class2       # folder containing documents of class 2
    │   │   └── classN       # folder containing documents of class N
    │   └── test 
    │       ├── class0       # folder containing documents of class 0
    │       ├── class1       # folder containing documents of class 1
    │       ├── class2       # folder containing documents of class 2
    │       └── classN       # folder containing documents of class N
1.	Download the repository
2.	Set your current working directory in .env file. It has 3 paths,
a)	raw_train_dir – put the path where the raw  train data(folder format) is saved .
b)	raw_test_dir – put the path where the raw inference data(folder format) is saved.
3.	Run the “folder_to_csv_conversion” to convert the above format files into CSV format.
4.	Once the CSV files are stored in the file path mentioned , Next steps would be following the same that has been done for CSV files.









































































