# Csv files in python
## Definition
A CSV file (Comma Separated Values file) is a type of plain text file that uses specific structuring to arrange tabular data. Because it’s a plain text file, it can contain only actual text data—in other words, printable ASCII or Unicode characters.

The structure of a CSV file is given away by its name. Normally, CSV files use a comma to separate each specific data value

The csv library provides functionality to both read from and write to CSV files. Designed to work out of the box with Excel-generated CSV files, it is easily adapted to work with a variety of CSV formats. The csv library contains objects and other code to read, write, and process data from and to CSV files.

## Reading Csv files
Reading from a CSV file is done using the reader object. The CSV file is opened as a text file with Python’s built-in open() function, which returns a file object. This is then passed to the reader, like this:

```
import csv,os
from pathlib import Path

def read_population(file_name):
    f = open(afile_name, 'r')
    csv_reader = csv.reader(f, delimiter=',')
    test_row_list = list()
    for row in csv_reader:
        test_row_list.append(int(row[0]))
    f.close()
    return test_row_list
```

## Writing Csv files
We can also write to a CSV file using a writer object and the .write_row() method:

```

import csv,os
from pathlib import Path

def write_answer(file_name,value):
    writeFile = open(file_name, 'w')
    writer = csv.writer(writeFile)
    writer.writerow([value])
    writeFile.close()
```

**Reference:**
- [https://realpython.com/python-csv/](https://realpython.com/python-csv/)