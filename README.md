# MEN-Dataset
(M)alaysian (E)nglish (N)ews Dataset with Annotated Entity and Relations. 

# Description
The Dataset includes 200 Malaysian English News Article with Human Annotated Entities and Relations. 

### Entities
The entity labels are adapted from OntoNotes 5.0 Dataset.
- PERSON
- ORGANIZATION
- LOCATION
- FACILITY
- EVENT
- WORK OF ART
- PRODUCT
- LAW
- NORP
- LANGUAGE
- ROLE
- TITLE

### Relations
The relation labels are adapted from DocRED and ACE05 Dataset. Please refer the document below for list of relation labels. 

[DocRED](./guideline/Relation%20Label%20Summary%20-%20DocRED.xlsx)
[ACE05](./guideline/Relation%20Label%20Summary%20-%20ACE05.xlsx)

# Guideline
Please refer to this documentation for the Full Annotation [Guideline](./guideline/Annotation%20Guideline%20v3.pdf). 
# Structure
The repository includes two folders, data and guideline. The data folder includes annotated file and the articles. The guideline file includes the Annotation Guideline used for this project. 

# Sample of Annotated Data
The sample below is taken from final annotated dataset. The id indicates the text file to refer for article. 
```json
{
  "id": "article_1",
  "entities": [
    {
      "id": 1,
      "label": "TITLE",
      "position": {
        "start_offset": 893,
        "end_offset": 895
      }
    },
    {
      "id": 2,
      "label": "PERSON",
      "position": {
        "start_offset": 116,
        "end_offset": 139
      }
    },
    {
      "id": 3,
      "label": "LOCATION",
      "position": {
        "start_offset": 0,
        "end_offset": 12
      }
    },
    {
      "id": 4,
      "label": "LOCATION",
      "position": {
        "start_offset": 14,
        "end_offset": 22
      }
    },
    {
      "id": 5,
      "label": "EVENT",
      "position": {
        "start_offset": 625,
        "end_offset": 633
      }
    }
  ],
  "relations": [
    {
      "id": 3,
      "head": 4,
      "tail": 3,
      "relation": "location",
      "relation_source": "DocRED"
    },
    {
      "id": 12,
      "head": 4,
      "tail": 5,
      "relation": "significant event",
      "relation_source": "DocRED"
    }
  ]
}
```
## License

[MIT](https://choosealicense.com/licenses/mit/)
