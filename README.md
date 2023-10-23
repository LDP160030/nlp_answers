# NLP_Exam
Showcase your NLP skills

Time taken to create & debug env dependencies(including cuda setup): 6hrs
Time taken to Q1: 4hrs, Q2: 2 hrs


Question #1 - Goal - train sentiment classifier

Use https://huggingface.co/datasets/FinanceInc/auditor_sentiment#data-fields dataset to fine-tune 
https://huggingface.co/roberta-base model



1. First freeze all the layers expect of classifier and tune head only (5.0)  -- 01-Training Sentiment dataset
2. Then unfreeze last 3 layers of the model and tune them (10.0) -- 01-Training Sentiment dataset
3. Evaluate finetuned model (5.0) --01-Training Sentiment dataset
4. Use Pipelines to create prediction pipline (5.0) --01-Training Sentiment dataset

Question #2 - Goal - Identify Top Keywords (See provided dataset in csv)

Questions to answer:
1. Please briefly describe your approach (10.0) -- Extracting top 10 keywords.ipynb
2. How did you define what “top” is? (5.0) -- Extracting top 10 keywords
3. List the top 10 keywords here along with the metrics. If you’d like to show us a visualization for it, you could do that (20.0) --Extracting top 10 keywords

4. If you were unable to complete your code in the allotted time, please describe what more you originally intended to implement. (5.0)
5. If you had a few weeks (say 4-8) to do this task, what other approaches would you try and implement for this problem? (10.0)


Q2)As there is no clear objective about the usecase except finding the topic 10 keywords. I plotted top tfidf importance by single word, 2-grams and 3-grams to understand words of importance in the documents.

Also, I trained gensim lda model in another notebook so as to find and visualize the important topics of the given documents. I would have tried finetuning lda model as well as training a ldamallet model if there is more time. Also, we could use the final topic keywords from each topic and summazing each topic keywords would actually give us a better understanding of what each topic is.


Q1)Sentiment model

If additional time were available, I could have conducted an in-depth error analysis on the sentiment model data/predictions and experimented with different threshold metrics to assess how the performance metrics change.

We have the flexibility to explore various hyperparameters, optimizers, and learning rates, while also considering different decay rates.

Given more time, I could have restructured the code into modular components for both the preprocessing, training and evaluation steps of the sentiment model. I would have implemented a custom pipeline.

