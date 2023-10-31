# Sentiment_Analysis_Fine_Tune
Fine Tuning Sentiment Analysis HuggingFace Model on FinGPT/fingpt-sentiment-train dataset

#First method includes creating a sentence classification pipeline which includes the following steps:
1. Creating a copy of "distilbert-base-uncased-finetuned-sst-2-english" from AutoModelForSequenceClassification class
2. Loading a tokenizer for the model from the model artifacts using the AutoTokenizer class.
3. Creating a Sentiment Analysis pipeline.
4. Classifying the trainig set of the data . 
<img width="470" alt="Screen Shot 2023-10-31 at 12 33 05 AM" src="https://github.com/aditii02/Sentiment_analysis_fine_tune/assets/38829128/c2fb189a-816a-471d-87a3-80a188f5e695">

#Second mehtod invloves fine tuning the model on yelp Review dataset which includes the following steps:
1. Preparing the dataset in two columns Review and label
2. Call tokenize on the whole dataset by using the map function which will tokenize the whole dataset.
3. Load the model and pretrained arguments which are needed to be trained.
4. Define a evaluation metrics to check the performance of the model in this case it will be Accuracy.
5. Call Trainer.train() from Pytorch and provide train_dataset,eval_dataset,compute_metrics in the arguments.
   

 




