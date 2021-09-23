# Computational Analysis of _Weird Fiction_ and _Eerie Fiction_
This repository contains all the relevant files about my Bachelor Thesis.
## Requirements
The following modules are necessary, they can all be installed using **pip install _name of the module_**.
* **stanza**    
The model for English language has to be downloaded once in a Python interpreter. This can be done like the following:   
``import stanza``  
``stanza.download("en")`` 
* **nltk**
* **pandas**
* **matplotlib**
* **sklearn**
* **tensorflow**
* **tensorflow_hub**
* **seaborn**
* **plotly**
## Corpus
The **plain** subfolder contains all single text files. The file _Corpus\_Overview.tsv_ contains all the data about the files, like author, title, translator, identifier etc.  
The identifier of each story is the file title. For example, the story _At the Mountains of Madness_ by H.P. Lovecraft has the identifier 3, and can be found as ```3.txt``` in the ```plain``` folder.
A more clearly arranged overview of the corpus can be found [here](https://docs.google.com/spreadsheets/d/1ba9V59JTGyw86F1YEwhSBCZFZR7UMYOxbvYgrtb8EM4/edit?usp=sharing).  
As control group, I also used the _webtext_ corpus that comes preinstalled with nltk.
## Code

```process_use_similarity.py``` in the _use_ subfolder creates the binary file ```similarities_dict``` in the _use_ subfolder. The file contains a dictionary with similarity scores
for every text in relation to all the other texts.  

``eerieness_measure.py`` creates the binary file ```someones_dict```, which contains a dictionary of the document titles (including the control group) as keys and their eerieness scores as values. 
It needs the following files:
* ``Corpus_Overview.tsv``
* ``latest_keyness_results_.txt`` in the _Keyness_ subfolder
* ``latest_keyness_results_swap.txt`` in the _Keyness_ subfolder
  
The _Keyness_ subfolder also includes the splitting of the files into eerie and reference corpus, for reproducability with Antconc. 
  
  
The jupyter notebook ``Display.ipynb`` visualizes the results of every method in plots and dataframes, more information can be found there.
