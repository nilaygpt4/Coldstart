# New Cold-Start Approach
- Taking the best of 2 Sentence Transformer models, namely all-mpnet-base-v2 and all-MiniLM-L12-v2, for each dataset. 

- Models fine-tuned with less than 5 samples per class, hence the training and inference is very time-efficient and resource-efficient as well (<20 sec). 

- MLP classifier fitted to the models, as it gives reasonably better metrics than Logisitic Regression and takes similar training time for smaller models and datasets.

## Dataset Legend

- cricket_trainset_fewshot, cricket_testset_mod: Slots Dataset
- labelled_data_fewshot, labelled_data_test_shot: AI-BR Test Dataset
- cricket_final_train_df_fewshot, processed_df_08-16-2021_13-21-00_sid_1675508193_dbsid_504: AI-BR Dataset provided by @Ambuje Gupta