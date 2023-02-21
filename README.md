# Extracting SMILE Structure and IUPAC Name of Drugs from PubChem using Drug Names

**Overview**
This Python script is designed to extract the SMILE structure of drugs from PubChem using drug names provided by the user. The user must submit a text file containing drug names separated by a new line. The code will automatically generate the SMILE structures of the respective drugs and save the output in a CSV file.

**Inputs**
A text file containing drug names separated by new line.

**Outputs**
A CSV file containing drug names and their respective SMILE structures and IUPAC names.

**Procedure**
1. The script starts by importing the necessary libraries, such as pandas, requests, and os.
2. The user is prompted to enter the name of the input text file containing drug names.
3. The script reads the input file and stores the drug names in a list.
4. For each drug in the list, the script searches for the compound in PubChem and retrieves its SMILE structure and IUPAC name.
5. The drug name and its corresponding SMILE structure and IUPAC name are exported as a CSV file. 
6. The output CSV file is saved in the resultant directory as the input text file.

**Assumptions**
1. The user has installed the necessary libraries (such as pandas, requests, and os).
2. The user has a stable internet connection to access PubChem.
3. The input text file only contains one drug name per line.
4. The drug names in the input file are spelled correctly and match the names in PubChem.

**Potential Improvements**
1. Add error handling to handle cases where a drug name is misspelled or not found in PubChem.
2. Add the option to output the SMILE structures in other file formats, such as SDF or Mol.
