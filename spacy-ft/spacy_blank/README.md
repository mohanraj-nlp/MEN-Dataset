
# spacy_blank

## Requirements and Installation

Python 3.10

Install libraries and dependencies

```python
  pip install -r requirements.txt
```

## Download Best Model
Download metadata [Google Drive](https://drive.google.com/drive/folders/1rgWAQ6NWk3JCXSk1RxN8uCOgLobVG1X_?usp=drive_link) for spacy_blank best model and put them into the current folder (spacy_blank).
## Usage/Examples

### Training (Optional)
```python
python -m spacy train config.cfg --output ./output --paths.train ./train.spacy --paths.dev ./dev.spacy
```
This will overwrite the existing model metadata that you have downloaded

### Validation
Run the Jupyter Notebook and read validation-spacy-format.json. This will allow to validate the model and provide NER performance metrics.

You may try with own sample of Malaysian English sentence if needed. 
