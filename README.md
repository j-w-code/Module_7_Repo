# *ETF Analyzer*
---

## ETF Analyzer
This project covers the use of the SQL database sytem and the hvplots library create ETF databases and plot the resulting data. 

>"Would you like to play a game?"

## Technologies 

This project uses Python, Pandas, Hvplot, and SQL database language to create databases, dataframes, and plot graphical interpretations of data. 

[pandas](https://github.com/pandas-dev/pandas)
[HVplot](https://github.com/holoviz/hvplot)
[SQLalchemy](https://github.com/sqlalchemy/sqlalchemy)

### Installation Guide

In order to use this program please import and utilize the following libraries and dependencies: 

```python
import numpy as np
import pandas as pd
import hvplot.pandas
import sqlalchemy
```

## Usage 
the following blocks of code from the Pandas library are fundamental in executing the program. 

```python 
database_connection_string = 'sqlite:///'
```
This creates a database connection string. 

```python
engine = sqlalchemy.create_engine(database_connection_string)
```
This command creates an engine for SQL to execute commands such as queries. 
```python
query ="""
SELECT *
FROM 
"""
```
This is a SQL query formatted as a string in python. It interacts with the engine to be processed. 
```python
df = pd.read_sql_query(query, engine)
```
This command converts the SQL query into a pandas dataframe for further data manipulation as needed.  
```python
df.hvplot(xlabel="",rot=, height=, width=, legend='').opts(yformatter='f',padding=())
```
This code will plot a graph of the dataframe containing the SQL data. It is modified by a yformatter and a padding option to increase visibilty of data.  

![<alt text>](https://i.postimg.cc/fRX2CHXK/ETF-Plot-Image.png)

## Contributors

Jeffrey J. Wiley Jr

## License

MIT



