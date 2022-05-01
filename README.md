# INST0075_Assessment2
#### 1. Install requirements:
- python 3.7
```python
pip install -r requirements.txt
python -m spacy download en_core_web_lg
```
#### 2. data
- The raw data of the paper is [Recipe1M+ dataset by Marin et al.](http://pic2recipe.csail.mit.edu) from http://im2recipe.csail.mit.edu/dataset/login/ (login required; the correct link is: Layers (381 MiB)). It's a dataset containing one million recipes with information like title, ingredient list, instructions, and images. Due to the large amount of data, we only secleted 1,000 instruction sentences for training models in this project. 
