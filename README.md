# Outlier row removal using inter quartile range

**Project 2 : UCS633 DATA ANALYSIS AND VISUALIZATION**


Submitted By: **Yash saxena 101703627**

***
pypi: <https://pypi.org/project/outlier-removal-yash-saxena>
<br>
git: <https://github.com/yashsaxena972/outlier-removal>
***

## IQR Interquartile range Description

Any data can be described by its five-number summary. These five numbers,consist of (in ascending order):

The minimum or lowest value of the dataset.
<br>
The first quartile Q1, which represents a quarter of the way through the list of all data.
<br>
The median of the data set, which represents the midpoint of the whole list of data.
<br>
The third quartile Q3, which represents three-quarters of the way through the list of all data.
<br>
The maximum or highest value of the data set.

## Calculation of acceptable data
```
IQR = Q3-Q1
lower=Q1-(1.5*IQR)
upper=Q3+(1.5*IQR)
```
The data values present in between the lower and upper are acceptable and the rest are outliers and hence being removed.

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install removal system.

```bash
pip install outlier-removal-yash-saxena
```

<br>

## How to use this package:

outlier-removal-yash-saxena can be run as done below:



### In Command Prompt
```
>> outliers <dataset.csv>
```
<br>


## Sample dataset

Marks| Students 
:------------: | :-------------:
3|S1
57|S2
65|S3
98|S4
43|S5
44|S6
54|S7
99|S8
1|S9


<br>

## Output dataset after removal 

Marks| Students 
:------------: | :-------------:
57|S2
65|S3
98|S4
43|S5
44|S6
54|S7

<br>

It is clearly visible that the rows S1,S8 and S9 have been removed from the dataset.


## License
[MIT](https://choosealicense.com/licenses/mit/)





