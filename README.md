# WaterQual
Nationwide Research on Drinking Water Analysis

## Motivation
The Environmental Protection Agency sets the maximum contaminant level (MCL) to protect public health and this study investigates the nationwide drinking water quality by a water quality index constructed from water sampling data at community water systems. The analysis can help assess current drinking water standards.

## Files
[webScrapeSystems](webScrapeSystems.ipynb): Web-scrape all zipcodes nationwide at United States Zipcodes (https://www.unitedstateszipcodes.org) and use the zipcodes to webscrape the water systems info at Environmental Working Group (https://www.ewg.org) and store the data in a local database.

[webScrapeSamples](webScrapeSamples.ipynb): Use the systems info from the local database to web-scrape water sampling records at Environmental Working Group (https://www.ewg.org) and store the data in a local database.

[CompileDatasets](CompileDatasets.ipynb): Combine datasets from years 2010 to 2015 and years 2012 to 2017.

[DataCleaning](DataCleaning.ipynb): Clean the data and filter for contaminants of interest.

[ModelTraining](ModelTraining.ipynb): Process the data further and train a model for prediction.

[Predictions](Predictions.ipynb): Load the trained model, make predictions, and merge the predictions back to the raw dataset.

### Key Takeaways and Notes
* Webscrape 30 million+ data and cope with HTTPError
* Log transformation to ensure prediction is above 0
* only 1% of predictions above the minimum reporting limit
* Analysis incoming
