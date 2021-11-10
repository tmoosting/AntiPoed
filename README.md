# AntiPoed 


## System Requirements
* python 3.6
* to run the notebook: jupyter

## File contents
* PoemGenerator.ipynb (contains the logbook and AntiPoed class)
* Little AntiPoed Poetry Collection: poetry book with 4 examples
* wordweb.png in /pics folder: Network graph for title page of the collection


## Running the application

Make sure you have all the files above & that your working directory is set where the above files are. 
If it's the first time you're running the application, make sure that it's called with `load_inspiring_set == True`. 

In PoemGenerator.ipynb run:
```
AP = AntiPoed()
AP.antipoed_poetry_collection(load_inspiring_set = True/False)
```
The environment variables of the AntiPoed class that can be tweaked are the following:

```
    poetry_collection_name: str = "Little AntiPoed Poetry Collection"
    len_poetry_collection: int = 4
    inspiree: str =  "edgar-allan-poe-poems" # inspiree
    inspirers: List =  field(default_factory=lambda: ["maya-angelou-poems", "oscar-wilde-poems"] )
    source_website: str = 'https://mypoeticside.com/poets/'  
    nlp_model =  spacy.load("en_core_web_lg")
    load_inspiring_set:bool = False
    size_inspiring_nouns_set: int = 1000
    size_inspiring_adjs_set: int = 1000
    size_inspiring_proper_nouns_set: int = 1000
```

