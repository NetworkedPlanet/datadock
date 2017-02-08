---
title: Selecting An Identifier
layout: page
order: 85
---

During the DataDock conversion process, each record in your spreadsheet is turned into an entity ready for use on the Web of Data. DataDock produces a page for every identity so that each entity in your dataset is accessible on the web.

As everything on the Web of Data has an address, DataDock produces an **identifier** using the row number of the record. If you wish to use a different column for use in the identifier, you can set this before you upload the data.

## Example

The default identifier uses the row number such as:
 `http://datadock.io/AwesomeDude/DemoRepository/survey-data.csv/_row=1`
 
If you have a column full of values that you would like to be used in the identifier instead of the row number (e.g. an column), then select it from the drop down list in the settings panel. 
  
 If the survey-data.csv spreadsheet in the example above has a "Survey ID" column, selecting it would produces identifiers such as:
  
 `http://datadock.io/AwesomeDude/DemoRepository/survey-data.csv/survey_id=1`
 
## Important Note
 
 The values from the column you choose for an identifier does not have to be numerical, but they **must be unique to that dataset**. It's also important that there are **no empty values** in the column you have selected to be in your identifiers. 