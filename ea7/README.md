# Tool Supported Data Cleaning

1. Clean the dsm-beuth-edl-demodata-dirty.csv mini csv from the first exercise with Trifacta Wrangler (if you have no cloud access use the download version).
Not the red bars that give you instant feedback (on big datasets) where errors could be!
Create a recipie to clean the data as good as you can (it must not be a general script). Try to upload only one file (e.g. with screenshots and the end result).

2. Load the Grid_Disruption_00_14_standardized - Grid_Disruption_00_14_standardized.csv Dataset from Kaggle: 15 YEARS OF POWER OUTAGES. Where are errors here? How would you clean this file?

## Exercise 1

### Upload CSV

![Initial CSV](./assets/1_inititalCSV.png)

### Creating a recipe to clean the data

![While cleaning](./assets/2_whileCleaning.png)

### Done

![Done](./assets/3_done.png)

[See new CSV](./assets/cleaned.csv)

## Exercise 2

### Errors

Die Spalten 'Time Event Began', 'Date of Restoration' und 'Time of Restoration' sind fehlerhaft.

- 'N/A' – Angaben löschen
- Daten in 'Time Event Began' und 'Time of Restoration' vereinheitlichen (z.B. nach Format: HH:MM)
- Daten in 'Date of Restoration' vereinheitlich (z.B. nach Format mm/dd/yyy -> analog zu 'Date Event Began')
- Anführungszeichen aus Spalten vom Typ String entfernen (kein direkter Fehler, aber unnötig)
- Spaltentypen 'Deman Loss' und 'Number of Customers Affected' in Integer ändern

![Errors](./assets/01_errors.png)
