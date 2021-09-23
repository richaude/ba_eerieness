# Computational Analysis of _Weird Fiction_ and _Eerie Fiction_
This repository contains all the relevant files about my Bachelor Thesis.
## Requirements
The following modules are necessary, they can all be installed using **pip install _name of the module_**.
* **pandas**
* **matplotlib**
* **seaborn**
* **plotly**
## Corpus
The **plain** subfolder contains all single text files. The file _Corpus\_Overview.tsv_ contains all the data about the files, like author, title, translator, identifier etc.  
The identifier of each story is the file title. For example, the story _At the Mountains of Madness_ by H.P. Lovecraft has the identifier 3, and can be found as ```3.txt``` in the ```plain``` folder.
An overview with sources for the stories used in the corpus can be found [here](https://docs.google.com/spreadsheets/d/1ba9V59JTGyw86F1YEwhSBCZFZR7UMYOxbvYgrtb8EM4/edit?usp=sharing).  
As control group, I also used the _webtext_ corpus that comes preinstalled with nltk.

## Visualization
  
  
The jupyter notebook ``Display.ipynb`` visualizes the results of every method in plots and dataframes, more information can be found there.
