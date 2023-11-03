# Python

- [gto76](https://gto76.github.io/python-cheatsheet)

## Books
- [Think Python](https://greenteapress.com/thinkpython/thinkpython.pdf)

## Documentation & Libraries

1. [Python Frameworks Overview](https://pythonframeworks.com/)
2. [Pandas](https://pandas.pydata.org/pandas-docs/stable/index.html)
3. [SQLAlchemy](https://stackoverflow.com/questions/53704187/connecting-to-an-azure-database-using-sqlalchemy-in-python)
4. [Python Docx](https://stackabuse.com/reading-and-writing-ms-word-files-in-python-via-python-docx-module/)
5. [PDF2DocX](https://dothinking.github.io/pdf2docx/quickstart.convert.html)
6. [OpenPyXl](https://openpyxl.readthedocs.io/en/stable/)
7. [PyIcloud](https://github.com/picklepete/pyicloud)

## Tutorials

1. [VENVs](https://realpython.com/python-virtual-environments-a-primer/)

### Connecting to a database
```python
import urllib
import pandas as pd
from sqlalchemy import create_engine
from sqlalchemy import text

server = 'mydatabase.here.windows.net'        # the location
database = 'MY_DB'                            # My DataBase
username = 'USERNAME'                         # USERNAME
port = str(1234)                              # PORTNUMBER
password = "*************"                    # PASSWORD
driver = '{ODBC Driver 17 for SQL Server}'    # this the dialect acording to https://docs.sqlalchemy.org/en/20/core/connections.html

connection_string_1 = 'DRIVER='+driver+';SERVER='+server+';PORT='+port+';UID='+username+';DATABASE='+ database + ';PWD='+ password
connection_string = 'mssql+pyodbc:///?odbc_connect=' + urllib.parse.quote_plus(connection_string_1)

engine = create_engine(connection_string)     # creates the engine and can be re-used to use this database

print("Engine:", engine)
```
