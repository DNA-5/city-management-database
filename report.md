# DnA Project Phase 4 Report

There are 8 top level commands, each for one requirement. Each of these top level commands has atleast 2 sub commands.

## `insert` - Commands to insert new data into the database

### New citizen

Inserts a new entry in the `Citizen` table, prompts for all the required details.

### New patient

Used to record a new patient, prompting for all the required details. This command modifies 3 tables.

### New loan

Used to record a loan, prompting for all the required details. There are 4 kinds of entities that a loan can go to, and in our model we have made the distinction by using 4 different tables. However this command modifies only one table at a time.

### Create bank account

Used to create a new bank account, prompting for all the required details. Modifies only one table.

### Record crime

Used to record a crime, prompting for all the required details. Modifies 4 tables.

## `update` - Commands to update existing rows in a table

### Update citizen income

Command used to update an citizens income if it changes. Prompts for citizen id, and new income.

### Update neighbourhood representative

Command used to update the representative of a neighbourhood. Prompts for pincode, and the citizen id of the representative.

## `delete` - Commands used to delete data from tables

### Clear citizen

Used to delete a citizen record. Before running this, the operator must make sure the citizen has been discharged from hospitals, cleared loans, etc.

### Clear patient

Used to delete a patient record when the patient is discharged.

### Clear loan

Used when a loan is cleared off.

### Remove bank account

Used when a bank account has to be closed down.

### Resolve crime

Used when a crime is resolved.

## `selection` - Used to select rows of interest

### Get people below an income

Prompts for an income level, and returns the ids and names of every citizen below this level.

### Get law enforcers

Gets ids and names of every citizen who works in an LEA.

## `projection` - Used to select columns of interest

### Get a projection of diseases

Lists all diseases the current patients are suffering from.

### Get a projection of crimes

List all charges that are currently a part of some crime report.

## `aggregate` - Aggregate functions used to get statistics of interest

### Get number of victims of a disease

Prompts for a disease and prints the number of people suffering from it.

### Get average tax per person

Calculates average income tax paid by all people of the city.

### Get LEA with highest budget

Prints all details of the LEA that currently has the highest budget.

## `search` - Utilites to search for data of interest

### Get all citizens in an apartment by search

Prompts for an apartment names, returns all records matching that apartment name.

### Search for parks by neighbourhood

Returns the details of all neighborhoods having a particular landmark detail (park).

## `analysis` - Some utilites that give out analysis by considering the relations between multiple entities

### Get crime rate by neighbourhood

Prints the neighbourhood details (along with the representative name) and the number of crimes happening in that neighbourhood.

### Get hospital count by neighbourhood

Prints the neighbourhood details (along with the representative name) and the number of hospitals for each neighbourhood.
