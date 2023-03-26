# MolecularDescriptors
Calculate molecular descriptors based on SMILES structure
This code is installing the padelpy library using pip and then using it to calculate molecular fingerprints for molecules in a CSV file named "fda.csv". The calculated fingerprints are then saved in another CSV file named "Molecular-fingerprint-FDA.csv".

The code first imports the required libraries - pandas and padelpy. It then reads the CSV file "fda.csv" using pandas' read_csv() function and stores it in a variable called "df".

The next few lines of code calculate molecular descriptors for a single molecule (the one in the first row of the "df" dataframe), using the from_smiles() function from the padelpy library. The resulting descriptors are then saved in a pandas dataframe called "descriptors".

The code then adds two columns to the "descriptors" dataframe, one for the SMILES string of the molecule and one for its zinc_id. The next few lines of code reorder the columns of the "descriptors" dataframe and save it in a new CSV file named "Molecular-fingerprint-FDA.csv".

Finally, the code loops over all the molecules in the "df" dataframe and calculates the molecular descriptors for each molecule using the from_smiles() function. The resulting descriptors are then saved in the "Molecular-fingerprint-FDA.csv" file, along with the SMILES string and zinc_id of each molecule. The progress of the loop is printed out after each iteration.
