**This repo is archived and has been moved.  [new repo location](https://github.com/qualia-insights/QIA)**

Qualia Insights Accounting System...why buy when you can write
your own system? My lovely Wife owns and operates a mental health
counselling business and I do her accounting.  For the last several
years I have used this simple Python script.  We bank with PNC so
it imports the CSV files and puts categories on everything.  The
system is not perfect so feel free to modify for your needs.

QIA is based on Python it runs on Raspberry Pi, Chromebook (using crouton with
Anaconda), iPad (using Pythonista), and MacOS (using Anaconda).  It is meant
to be run from the iPython prompt interactively. All the modules used are well
known and easy to install. The list of Python dependencies are:
* matplotlib
* numpy
* Python Standard Library modules: CSV, datetime, os

# General Steps

0. Export the month's bank account information from PNCBank.com

1. set the variable path_to_data
```python
path_to_data = '/home/pi/qualia_insights_accounting' + "/data/2017"
```

2. run QIA.py in iPython...note nothing will run it will just load
the functions in QIA.py.

3. load the csv data
```python
bank_data = load_csv_data(path_to_data)
```

4. Read the categories csv file
```python
categories = read_categories("/home/pi/qualia_insights_accounting/data/categories.csv")
```

# To-Do List


0. Generate monthly reports print out in html

1. Generate yearly reports print out in html

2. Save graphs as images then place into reports

3. Make a different in transactions for personal and business.  For example
we might have an expense that is paid with personal.  I am thinking have
different names for the data files.

