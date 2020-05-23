# Python 4

## Exercise
1. Set up your Jupyter Notebook. Either by hand or by Anaconda. Play with it and send me the *.ipnyb or better (a GitHub) link to it.

### Result

```zsh
sudo python3 get-pip.py
pip3 install --upgrade pip
python get-pip.py pip==20.0.2
pip3 install jupyter pandas --user
jupyter notebook
```

2. Read the first 25 Exercises from 101 NumPy Exercises. (Prove is the string you send to me: Write "I read the first X (X>=25) exersises" ;-)

```I read the first X (X>=25) exercises```

3. Do the following exercise in a Jupyter Notebook (a GitHub Link would be the best):
    * Load the countries.csv directly via URL import into your panda data frame!
    * Display some basic information as rows, columns and some basic statistical info.
    * Show the last 4 rows of the data frame.
    * Show all the row of countries who have the EURO
    * Show only name and Currency in a new data frame
    * Show only the rows/countries that have more than 2000 BIP (it is in Milliarden USD Bruttoinlandsprodukt)
    * Select all countries where with inhabitants between 50 and 150 Mio
    * Change BIP to Bip
    * Calculate the Bip sum
    * Calculate the average people of all countries
    * Sort by name alphabetically
    * Create a new data frame from the original where the area is changed as follows: all countries with > 1000000 get BIG and <= 1000000 get SMALL in the cell replaced!
