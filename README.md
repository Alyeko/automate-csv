# automate-csv
Python code to automate the (mundane) task of editing coordinates stored in a csv before being uploaded unto a spatial database. 

One function which: 
1. Takes filepath as argument
2. Looks for all csv files in a filepath and reads them as pandas dataframes
3. Deletes rows labelled as 'REF' and 'CLO'
4. Deletes third and fourth columns which contain height coordinates and 'REF' and 'CLO' strings respectively
5. Sorts dataframe by first column
6. Saves dataframe as csv at the same filepath and overwrites the old one which was initially read (but this would depend on the name of your input csvs)

## Running the code (Experiencing the magic):
1. The code is best run in the same folder where your csvs are stored
2. Simply run the code in a jupyter notebook, IDE of your choice or terminal

## Assumptions made
1. The exact labels 'REF' and 'CLO'

## Problems to tackle/fix:
1. Sorting the first column(name of point)
 
## Things to add:
1. Regex for other variations of 'REF' and 'CLO'
2. If the csvs are not all in one folder
3. Gui(PyQt5) for non-python users
