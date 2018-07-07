Qualia Insights Accounting System...why buy when you can write
your own system?

QIA is based on Python running on the Raspberry PI.  It is meant
to be run from the iPython prompt interactively.  

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

1.5 Save graphs as images then place into reports

2. Make a different in transactions for personal and business.  For example
we might have an expense that is paid with personal.  I am thinking have
different names for the data files.

Test this change to see if it goes back to Pi and Mac! How do I get this changes staged?

ok this change is from working copy on iPad, which I am not sure if I need this app since
I can use stash?


