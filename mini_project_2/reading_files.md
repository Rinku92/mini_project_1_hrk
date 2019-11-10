# Reading Files
## Definition
There is no need for importing external library to read and write files in Python.  Python provides an inbuilt function for reading files.

## Reading a file

```
def read_csv(self):
    f=open("abc.txt", "r")
	if f.mode == 'r':
		contents =f.read()
	print(contents)
```

## Read a file line by line

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

**Reference:**
- [https://www.geeksforgeeks.org/constructors-in-python/](https://www.geeksforgeeks.org/constructors-in-python/)