# python-homework
Unit 2 | Homework Assignment: Automate Your Day Job with Python

# Import pathlib and csv
from pathlib import Path
import csv

# connect variable to csv
csvpath = ('budget_data.csv')

# decalre variables
average_change = 0
tot_months = 0
tot_dollars = 0
most_increase = 0
most_decrease = 0

# open csv
with open(csvpath, 'r') as csvfile:
    csvreader = csv.reader(csvfile)
    csv_header = next(csvreader)
    data = list(csvreader)
  
    print(data[1])
