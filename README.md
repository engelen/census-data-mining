Data mining assignment for LIACS Databases and Data Mining course. This public repository contains three main parts: the original Census adult data set, the WEKA Knowledge Flow for generating results, and the Python code for parsing the results and calculating interestingness measures. The following steps can be taken to run the experiments.

####Step 1
#####Running WEKA Knowledge Flow to preprocess and find potentially interesting association rules
The WEKA Knowledge Flow files are located in the directory `KnowledgeFlow`. To run the Knowledge Flow, simply import it in the WEKA KF environment and open the Census data set csv file, which is located in the `/Datasets/Census` folder. Running the knowledge flow will output directly to the `KnowledgeFlow` directory. The resulting rules cannot be written to a file by WEKA, and must be manually saved into `results.txt` in the `KnowledgeFlow` directory. The `kf_data.csv` file contains the preprocessed data.

####Step 2
#####Computing interestingness measures
The output from WEKA can be used directly in the Python interestingness calculation script. Simply running `Interestingness/main.py` will generate a JSON file `rules.json` containing relevant information for all rules found by WEKA.
