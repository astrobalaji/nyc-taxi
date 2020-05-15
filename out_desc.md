# NYC taxi regression model

## Description of the data
Out of 17,617 records about 16,000 records which are useable for further training. Description of the errors on data can be found in 'Explore & Clean.ipynb'

The weather description is encoded two techniques 

* scikit-learn LabelEncoder routine
* spacy pre-trained vectors


## Description of the data files

* nyc_taxi_data.csv : The raw data about the New york taxi traffic with weather data
* faulty_records.csv : The faulty records detected from 'Explore & Clean.ipynb' notebook
* cleaned_data_spacy.p: The cleaned data with word embeddings of the weather description
* cleaned_data.csv: The cleaned data with a Label encoding of the weather description


## Description of the Notebooks

* Explore & Clean.ipynb : Data Exploration, Clean up and preparation for model training. 
* Keras train.ipynb : Training a simple LSTM model with the cleaned data (Label encoding for the weather description)
* Simple Regressor Train.ipynb : Training couple of simple regression models from scikitlearn (Spacy word embedding for weather desciption)

## Downloading spacy models

Before executing the spacy embeddings model, please execute the following in the terminal


```bash
python -m spacy download en_core_web_sm
```