# Tachyus UX/UI Coding Challenge
The Tachyus UX/U Coding challenge, provides Tachyus with the ability to test your knowledge, skills and ability to take instruction when developing software. For this challenge you will need to demonstrate the following 

1. An ability to develop a single page application using react, typescript, and css.
2. Visualize the information provided by the Completion and Production csv files.  
3. Provide the ability to search and sort the information associated with files
4. Provide functionality to update a record in the production file and demonstrate the change in the visualization



## Some helpful hints before yous start
These are just helpful suggestions, you _do not have to use them_

1. For parsing the csv file you might want to use https://www.papaparse.com/
2. For controls, tables, and other UI elements you could use https://blueprintjs.com/
3. For visualization you could use [recharts](https://github.com/recharts/recharts), [victory](https://github.com/FormidableLabs/victory), [nivo](https://github.com/plouc/nivo), [react google charts](https://react-google-charts.com/)



### Files
The files you will need to use are the completions and production files listed below. They are simple csv files with a defined relations.


#### Completions
This file include completion information for demo field we would like to evaluate. 

##### Columns
|wellName|wellAPI|boreID|compSubId|X|Y|TD|IsHorizontal|reservoir|faultBlock|compartment|maxBHP|long|lat|
|--------|-------|------|---------|-|-|--|------------|---------|----------|-----------|------|----|---|

##### Source
[https://github.com/Tachyus/coding-challenge/files/7695818/completions.csv](https://github.com/Tachyus/coding-challenge/files/7695818/completions.csv)




#### Production
This file includes production information for demo field we would like to evaluate. 

##### Columns
|year|month|wellAPI|boreID|completionGroupSubId|bhp|oil|water|gas|waterInj|compl|flowDays|pressure|status|
|----|-----|-------|------|--------------------|---|---|-----|---|--------|-----|--------|--------|------|


##### Source
[https://github.com/Tachyus/coding-challenge/files/7695821/production.csv](https://github.com/Tachyus/coding-challenge/files/7695821/production.csv)
