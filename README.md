# README

## Setup

### IPython###
* Requires a recent installation of IPython Notebook on the local machine.
* The [Anaconda Python distribution](http://continuum.io/downloads) includes a suitable version.

### Spark###
* Requires [Apache Spark](https://spark.apache.org/) version 1.3 or above.
* The startup script (see below) assumes Apache Spark has been installed in $SPARK_HOME on your local machine.

### Sample data###
* This exercise uses a sample CSV file of the latest monthly "price paid data" for house sales from the UK Land Registry.
* This sample file is in the `/data` directory.
* You can also [download the latest version of the monthly PPD CSV file](http://publicdata.landregistry.gov.uk/market-trend-data/price-paid-data/a/pp-monthly-update-new-version.csv) (usually around 14MB) directly from the Land Registry website. 
* Other data formats are [also available for download](http://data.gov.uk/dataset/land-registry-monthly-price-paid-data).
* The CSV files do not contain the column definitions, but [these are defined on the Land Registry website](https://www.gov.uk/about-the-price-paid-data)

#### Data licence####
* The UK Land Registry data is [published under specific licence conditions](https://www.gov.uk/government/statistical-data-sets/price-paid-data-downloads#when-using-or-publishing-our-price-paid-data)
* Attribution for UK Land Registry data:  Data produced by Land Registry (c) Crown copyright 2015.

## Starting the IPython Notebook##
* There is a script to start the notebook on a Linux platform:
`start_notebook.sh`
* If you are on a different operating system, check the Apache Spark Python documentation for your system.

## What the notebook does##

* In this demo notebook, we load up a file of sample CSV data on house sales from the UK Land Registry.
* Next we apply a Spark SQL table definition over the data.
* Then we perform some simple aggregation queries using both the older API and the new DataFrame functions.  
* This is just a quick experiment, but my impression is that the DataFrame API queries are significantly faster than the older equivalents.
* You can play around with the queries to explore the data and the APIs for yourself.

## Licence##

* [Apache Spark](http://spark.apache.org/) is licenced by the Apache Software Foundation.
* See the [Anaconda website](https://store.continuum.io/cshop/anaconda/) for details of Anaconda licencing.
* See the [IPython website](https://ipython.org) for details of IPython licencing.
* See the [UK Land Registry website](https://www.gov.uk/government/statistical-data-sets/price-paid-data-downloads#when-using-or-publishing-our-price-paid-data) for details of the licence covering the  sample CSV data used here. 
* The following licence applies *only* to the notebook code in this sample application:
---
The MIT License (MIT)

Copyright (c) 2015 Christopher M.H. Webster

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.