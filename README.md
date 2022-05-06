# Food2vec and Foodbert for Food Ingredient Substitution
### <center> Student Number: 21070178 &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; Lecturer: Dr Luke Dickens</center>  
### <center> INST0075: Machine Learning Methods &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; &ensp; Assessment: Report </center>
#### 1. External libraries
- python 3.7
```python
pip install -r requirements.txt
python -m spacy download en_core_web_lg
```
#### 2. data
- The raw data of the paper is [Recipe1M+ dataset by Marin et al.](http://pic2recipe.csail.mit.edu) from http://im2recipe.csail.mit.edu/dataset/login/ (login required; the correct link is: Layers (381 MiB)). It's a dataset containing one million recipes with information like title, ingredient list, instructions, and images. Due to the large amount of data, we only secleted 1,000 instruction sentences for training models in this project. 
- The data we used is Recipe1K, which is sampled from Recipe1M+, is provided in data/normalization folder.
- We  use an ingredient dataset provided by Yummly (Yummly, 2015) as the starting point to create a list of all ingredients. it's provided in data/normalization folder.
- The ground truth file 'ground_truth_substitutes_dict.json' is not open to public, I contacted the author to obtain this file only use for this assessment.
#### 3. Download the Bert models
- Download https://github.com/ChantalMP/Exploiting-Food-Embeddings-for-Ingredient-Substitution/releases/download/0.1/foodbert_data.zip， unzip it and place the 'mlm_output' folder in ./data.
- Download https://github.com/ChantalMP/Exploiting-Food-Embeddings-for-Ingredient-Substitution/releases/download/0.1/foodbert_embeddings_data.zip unzip it and place the file ‘food_embeddings_dict_foodbert.pkl’ in ./foodbert_embeddings/data
