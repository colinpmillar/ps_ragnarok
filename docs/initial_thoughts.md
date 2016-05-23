
![](http://www.ices.dk/_layouts/15/1033/images/icesimg/iceslogo.png "ICES")

# Streamlining recurrent assessments

## Core issues we are addressing

* reproducability
* transparency
* data quality
* efficient time use

## Project/framework design guide

* Encapsulated framework
* use existing procedures and processes
* designed flexibility

## percieved/hoped for benefits

* more time for experts to spend on problem solving
* more control over inputs and outputs

## constraints

* deliver in 2 years
* minimal upkeep?

## wider issues

* buy in by stock assessors
* issues with ownership of assessments and process
* the variety of approaches
* how much standardisation to apply / impose
* who updates the procedures at benchmark?
* user freindly

# Scoping

## The system **will**
* work for all stock assessment
* allow assessments to be rerun quickly and automatically
* allow alternative assessments to be archived (i.e. allow multple assessment runs)
* provide a way to track changes in input data from year to year
* provide a way to track changes in assessment scripts from year to year
* require experts to use R in thier stock assessments

## The system **will not**
* archive user code for ad-hoc analyses

## The system **might**
* allow users to work from their own hard drives
* allow users to use different analysis software?


# Requirements


## Databases
* new database of stock assessment inputs
* new database of stock assessment outputs
* new database/archive of stock assessment methods

### input database requirements
* read from DATRAS
* read from intercatch
* read from RDB
* experts can add survey and catch data
* perform data checks on expert data
* accessible via webservice and ideally with a "view" that looks like a directory structure of csv files

### output database requirements
* accessible via webservice and linked to input data csv view (above)

### method archive requirements
* can hold code
* can hold executables
* archives previous versions of R
* archives previous g++ and gfortran compilers

## servers
* server to read data, load model, run model and output results
* server to hold databases

### requirements
* read data from other ICES databases via webservices
* run compilation scripts
* run executables
* output data to a database

