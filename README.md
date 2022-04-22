# Tachyus UX/UI Coding Challenge
The Tachyus UX/U Coding challenge, provides Tachyus with the ability to test your knowledge, skills and ability to take instruction when developing software. For this challenge you will need to demonstrate the following.

1. An ability to develop a single page application using [React](https://reactjs.org/).
2. Visualize the information provided by the Completion and Production csv files.  
3. Provide the ability to search information associated with files.
4. Provide functionality to update a record in the production file and demonstrate the change in the visualization.



## Some helpful hints before yous start
These are just helpful suggestions, you _do not have to use them_

1. For parsing the csv file you might want to use https://www.papaparse.com/
2. For controls, tables, and other UI elements you could use https://blueprintjs.com/ or https://mui.com/
3. For visualization you could use [recharts](https://github.com/recharts/recharts), [victory](https://github.com/FormidableLabs/victory), [nivo](https://github.com/plouc/nivo), [react google charts](https://react-google-charts.com/), or [d3](https://d3js.org/)
4. Use create react app and yarn


## SourceFiles
The files you will need to use are the completions and production files listed below. They are simple csv files with a defined relations.


### Completions
This file include completion information for demo field we would like to evaluate. 

#### Columns
|wellName|wellAPI|boreID|compSubId|Type|X|Y|TD|IsHorizontal|reservoir|faultBlock|compartment|maxBHP|long|lat|
|--------|-------|------|---------|----|-|-|--|------------|---------|----------|-----------|------|----|---|

#### Source
[https://github.com/Tachyus/coding-challenge/files/7695818/completions.csv](https://github.com/Tachyus/coding-challenge/files/7695818/completions.csv)


### Production
This file includes production information for demo field we would like to evaluate. 

#### Columns
|year|month|wellAPI|boreID|completionGroupSubId|bhp|oil|water|gas|waterInj|compl|flowDays|pressure|status|
|----|-----|-------|------|--------------------|---|---|-----|---|--------|-----|--------|--------|------|


#### Source
[https://github.com/Tachyus/coding-challenge/files/7695821/production.csv](https://github.com/Tachyus/coding-challenge/files/7695821/production.csv)

### Relationships
These files are related to each other by the following column definitions.

|Completions Column|   |Production Column   |
|------------------|---|--------------------|
|wellAPI           | = |wellAPI             |
|boreID            | = |boreID              |
|compSubId         | = |completionGroupSubId|

# The Challenge
Please review the following steps and let us know if you have question of need clarity.

You will need first initialize your project, get it ready to build and make sure it can be ran on localhost. 

## Step one - Display data from file
For this step you will load and display the information from the provided files.

1. Load the [completions](https://github.com/Tachyus/coding-challenge/files/7695818/completions.csv) and the [production](https://github.com/Tachyus/coding-challenge/files/7695821/production.csv) files.

2. Using the files you will display the information in a grid from the production file.

3. **(Bonus)** In addition to these columns, you could add a Gross column which is oil + water.

## Step Two - Visualize data from file
For this step you are going to add a visualization for the data, this visualization should be displayed along with the grid. 

1. Using a graphing library, add a timeseries line graph showing oil, water, gas, and waterInj rate over time.

## Step Three - Searching the data in the files
For this step you will provide the user with an ability to search the data for a specific wellName, the search should give the user the option to use partial names. 

*Example:* If the user types _PLMS_ in the search input, the page will filter to only show wells that start with _PLMS_.

1. Add a search input box to the page. 

2. The search functionality may be triggered by the user's typing or by the user hitting a search button. It needs to do one but does not need to do both. 

3. The grid and visualization must filter to only show the data associated with the results from the search input.

## Step Four - Updating a wells name
For this step you will give the user the ability to edit the name of one of the wells in the grid. 

1. Provide the user with the ability to select a well from the grid.

2. Once the user has selected a well give them the option to change the name and save.

3. The name change should be reflected in the grid and in the visualization. 

## Bonus - Add a map
This is a bonus, since the completion data has lat and long, use a mapping library like google maps or mapbox to show the location of the wells.

1. Display the well location markers on a map for the corresponding rows in the completions file. 

2. The based on the type of well, show a different marker icon or color. For example producers can be green and injectors could be red. 

3. Add a tool tip, to the marker displaying the information about the well like wellName, Type, TD,....


# Submitting your work
Once you have completed as many steps as you can, please submit your work to a public github or bitbucket account and share the link with Tachyus for review. 

Have fun and don't get stressed. 
*Tachyus Engineering Team*

## Note
You don't have to complete all of the steps in the time you where given.
