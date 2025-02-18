# Frugal AI Climate Disinformation

## Frugal AI challenge

This repository contains work related the Frugal AI Challenge 2025

The goal of the Frugal AI challenge was to obtain the highest possible accuracy, with the lowest energy consumption. 
There were three possible tasks (source: https://frugalaichallenge.org/about/) 
1. Detecting climate disinformation: based on text from news articles.
2. Classifying regions at risk of wildfires: based on image data gathered via satellite.
3. Detecting illegal deforestation : from bio-acoustic data recorded in the jungle.

But this repository focuses on the **text challenge**. 


## Folder Structure 

The structure of the folder is as follows: 

- `0_EDA`: Contains Exploratory data analysis performed on the dataset. 
- `1_data_augmentation`: Contains data augmentation performed using back-translation. 
- `2_baseline`: Contains baseline models predicting a binary classification (climate disinformation presence/absence) or a multi-class classification (random class). 
- `3_unsupervised_models`: Contains centroid similarity and KNN models. 
- `4_bert_models`: Contains RoBERTa, DistilBERT and ModernBERT models. 
- `5_best_performing_model`: Contains our best-performing model, a fine-tuned ELECTRA MODEL. 

## Results 

Our best-performing model, the ELECTRA fine-tuned model (12 unfrozen layers) with obtained the following results: 

|Accuracy| Energy consumed (Wh)|
|--|--|
|0.73|0.94| 



## 📂 Cloning the Repository  

Since this project includes a **Git submodule** (the `Submission` folder linked to a private Hugging Face Space), follow these steps to ensure everything is cloned properly:

### **Clone with Submodules**
To clone this repository along with its submodules, run:  
```bash
git clone --recurse-submodules <https://github.com/JulianaGomez/frugal_ai_climate_dissinformation.git>