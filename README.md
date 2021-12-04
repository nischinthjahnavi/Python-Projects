# SQL Functions in Python

The objective of this project is to execute sql operations and data manipulations using python code by establishing a connection between Python and MySQL application

## Getting Started

Select the Code dropdown button highlighted in green for the required branch. Out of all options provided, choose the last option to download the zip file of the python code.
Start an instance of Anaconda distribution running and launch Jupiter Notebook

### Prerequisites

To execute the sql functions in python, the following software should be installed and ready for use

* [Anaconda](https://www.anaconda.com/products/individual) - Used to install the Anaconda distribution platform

* [MySQL Workbench](https://dev.mysql.com/downloads/workbench) - Used to install the MySQL workbench in Windows OS for desktop and Laptop

* [Video game sales](https://www.kaggle.com/gregorut/videogamesales) dataset should be already present as a table in database

### Installing  

Follow the below steps to install the latest version of Anaconda in our local machine

1) Go to the Anaconda website for downloads - https://www.anaconda.com/products/individual (the Anaconda installers will be near the bottom of the page)
2) Download the appropriate latest version of Anaconda
3) After your installation is complete, verify it by opening Anaconda Navigator: 
4) On a Windows PC, from the start menu, select Anaconda3(64-bit), then select Anaconda Navigator. If Navigator opens, you have successfully installed Anaconda. 
5) Now close the Anaconda Navigator application
6) Open Windows PC open the Anaconda Prompt (start menu under Anaconda3(64-bit)) 
7) Enter the following commands one at time and wait for each install to complete running.
```
pip install plotly
pip install imbalanced-learn
pip install mlxtend
pip install pandas-profiling
pip install Boruta
```
8) Close the Anaconda Prompt/Terminal App and then restart to launch Jupiter notebook

Follow the below steps to install the latest version of MySQL workbench in our local machine

1) Go to the MySQL website for downloads https://www.mysql.com/downloads/
2) Select the right installer for Windows and download the same
3) After the download, open the installer
4) Select the right setup type based on your preference
5) Go with the default setting for configuration and click Next
6) For authentication, use a strong recommended password encryption
7) Go with the default configuration setting and complete the installation
8) Now launch the MySQL Workbench and the MySQL Shell

## Implementation Details

The objective of this python code is to execute simple database queries and aggregate functions with filtering using python instead of regular relational database.
The aim of this python code is to find out whether the average global sales of video games before 2005 was higher or after 2005 using 2 ways.

Method 1: Enclosing the SQL query containing groupBy aggregate function and case-when function
```
a) Install the mysql-connector-python using pip install command which will help connect python with mysql
b) Import numpy, mysql.connector and panda libraries in order to implement the right method for sql operations required
c) Load the video game sales data into a mysql workbench in a separate table
d) Read the video game sales data into using sql.connect() to establish a connection between the database and python
e) Keep the credentials like username and password are kept in a separate text file to avoid privacy breach
f) pd.read_sql() is used to read any query passed to it along with the connection object. 
g) The average global sales for pre-2005 and post-2005 years are displayed.
```

Method 2: Using groupby (), and mean () function on the dataframe object
```
The steps to execute this method is almost same as compared to method 1.
The only difference is that instead of using sql.connect(), we use simple groupby method on Sales data
Then finally apply mean() on the global sales data alone
```
We also use the where condition on the data frame to filter video games sales before and after pre-2005 and post-2005 value in a new column


## Built With

* [Python](https://www.python.org/downloads/release/python-3810/) -The version 3.10 has more features, online documentation and community support
* [Jupiter Notebook](https://jupyter.org/install) - This is an open source cloud based platform where users can edit the document and interpret the sales faster

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Jahnavi Nischinth** - [Python Projects](https://github.com/nischinthjahnavi/Python-Projects)

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE.md](LICENSE.md) file for details
## Acknowledgments

* I would like to acknowledge Gregory Smith who provided the dataset for video game sales data from 2016
