# automate-csv
Python code to automate the (mundane) task of editing coordinates stored as csvs before being uploaded unto a spatial database. 

One function which: 
1. Takes filepath as argument
2. Looks for all csv files in a filepath and reads them as pandas dataframes
3. Deletes rows labelled as 'REF' and 'CLO'
4. Deletes third and fourth columns which contain height coordinates and 'REF' and 'CLO' strings respectively
5. Sorts dataframe by first column
6. Saves dataframe as csv at the same filepath and overwrites the old one which was initially read

## Running the code (Experiencing the magic):
Open a terminal and run the following...
1. python3 -m venv venv
2. source venv/bin/activate
3. pip install -r requirements.txt
4. python downloader.py

## Assumptions made
1. The exact labels 'REF' and 'CLO'
 
## Things to add:
1. Regex for other variations of 'REF' and 'CLO'
2. If the csvs are not all in one folder
3. Gui(PyQt5) for non-python users
