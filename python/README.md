# deid-Shaojun Yu.py
Python code for de-identifying electronic medical records
# Prerequisites
## Python
* Python 3.5
* NLTK package for Python

 Running insturctions
## Python Code
### De-identification
1- Change to the python directory

2- uncomment a function  in ```deid()```  
```! make sure to uncommnet only one function each time```  
```! Do not run all functions at once```
```
# pass all to check_for_phone to find any phone numbers in note.
# check_for_phone(patient,note,chunk.strip(), output_file)
# check_for_Date(patient,note,chunk.strip(), output_file)
# check_for_PTName(patient,note,chunk.strip(), output_file)
  check_for_age(patient,note,chunk.strip(), output_file)
# check_for_HCPName(patient,note,chunk.strip(), output_file)
# check_for_RelativeProxyName(patient,note,chunk.strip(), output_file)
```

2- run ```python deid-Shaojun Yu.py id.text phone.phi```

In which:

* ```id.text``` contains Patient Notes.
* ```phone.phi``` is the output file that will be created.
### Stats
1- change to the python directory

2- run ```python stats.py id.deid id-phi.phrase phone.phi ```

In which:

* ```id.deid``` is the gold standard that is category-blind.
* ```id-phi.phrase``` is the gold standard with the categories included.
* ```phone.phi``` is the test file that the stats is run on.
