
# spacy_en_core_web_trf

## Requirements and Installation

Python 3.10

Install libraries and dependencies

```python
  pip install -r requirements.txt
```

## Download Best Model
Download metadata [Google Drive](https://drive.google.com/drive/folders/12C1byjELvAvUYm7Z9_vDidbcD9bjRXBH?usp=share_link) for spacy_blank best model and put them into the current folder (spacy_en_core_web_trf).
## Usage/Examples

### Training (Optional)
```python
python -m spacy train config.cfg --output ./output --paths.train ./train.spacy --paths.dev ./dev.spacy
```
This will overwrite the existing model metadata that you have downloaded

### Validation
Run the Jupyter Notebook and read validation-spacy-format.json. This will allow to validate the model and provide NER performance metrics.

You may try with own sample of Malaysian English sentence if needed. 