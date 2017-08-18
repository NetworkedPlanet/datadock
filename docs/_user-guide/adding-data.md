---
title: Adding Data
layout: page
order: 40
---

This document describes the import interface for adding data to DataDock.
For a quick guide on how to import data, please read the [Getting Started Guide](../getting-started/).

## Procedure

The basic procedure for adding data to DataDock is quite simple. You must be 
[logged in](./logging-in-and-out.html) to the DataDock portal to perform this action. 
You can access the interface to add data from your Dashboard page by clicking on the `Add Data` button.

### Select File To Import

The first step in the import process is to choose the file to import. The [Getting Started Guide](../getting-started/)
has some useful hints on what the content of this file should be, but the most important restrictions are:

  - It must be a CSV file using commas (,) as the separator
  - It must be no more than 4MB in size
  - The file name must be no longer than 40 characters
  
To select the file to import click on the Browse button and use the dialog that appears to find and select the CSV file to import.
Once you select the file to import, the content is read locally (it is not uploaded at this point), and the screen changes
to allow you to review and modify details before the upload and conversion process starts.

### Update the Metadata

By default the dataset will use the file name as it's title. We strongly recommend that you change this default **title** to something more meaningful. You can also enter **description** text to help other users understand what is contained in 
your data. If you are publishing data that comes from a dataset whose license stipulates attribution, place this attribution in the description field.

You must select a license from one of the the four license options. The license options are:

  * [CC-0](https://creativecommons.org/choose/zero/) - A Creative Commons license that frees your work of copyright restrictions around the world. 
  
  * [PDDL](https://opendatacommons.org/licenses/pddl/1.0/) - The Public Domain Dedication & Licence from the Open Data Commons allows others to freely share, modify, and use your work for any purpose and without any restrictions. 

  * [CC-BY](https://creativecommons.org/licenses/by/4.0/) - A Creative Commons license that requires users to give attribution to you and to indicate if any changes where made. It allows sharing, reuse and transformation of your data for any purpose, including commercial purposes.
  
  * [OGL](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/) - A license similar to the Creative Commons CC-BY license, widely used in UK Government open data initiatives. This license requires attribution, but it does not require that derived datasets be published as open data.

  * [CC-BY-SA](https://creativecommons.org/licenses/by-sa/4.0/) - A Creative Commons license that requires users to give attribution to you and to indicate if any changes were made. It allows sharing and allows reuse and transformation of your data for any purpose, including commercial purposes as long as the results are distributed under the same license as your data.

  * [OGL](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/) - A license similar to the Creative Commons CC-BY license, widely used in UK Government open data initiatives.

We recommend using CC-0 whenever possible as this provides the most freedom and places the least restrictions on the use and reuse of your data. However
you should ensure that you comply with the licensing terms of any source data you have used to create your data as well as with the policies of your
organisation.

**NOTE** - we are aware that there are many other licenses available, we have tried to keep the choice as simple as possible. However we [welcome feedback](https://github.com/NetworkedPlanet/datadock/issues)
on other licenses that we should consider adding support for.

### Add Tags

You may choose to add any number of keyword tags to your dataset in the `Tags` field. As you type in this field, pressing either comma (,) or Enter on your keyboard will create a separate keyword.

We recommend at least tagging the content with the subject of the data. You may want to also consider tagging it with the geographical region(s) to which the data applies.


### Review and Update Column Datatypes (Column Definitions Tab)

The DataDock script will attempt to determine what kind of data is provided in each field by examining the first row of data following the column headers.
From this it will set an initial datatype for each column - this is the definition of what format of data is held in the column. The supported datatypes are:

  - **Text** - for basic text content
  - **URI** - for web links
  - **Whole Number** - for integer values (numeric data without any decimal points)
  - **Decimal Number** - for decimal values (numeric data where the data may include a decimal point)
  - **Date** - for date values without any time component
  - **Date And Time** - for date values that include a time component
  - **True / False** - for boolean values such as "true" and "false", "T" and "F", "1" and "0"
	
For more details about the different datatypes and how they are processed during the conversion, please see the [Datatypes](./datatypes.html) article.

### Choose the Identifier Column (Advanced Tab)

Each row in your CSV file will get a unique identifier generated for it during the conversion process. By default, this identifier is generated from the name of the CSV file you have uploaded and the row number of the row. However, often a dataset will contain a column that provides a natural identifier to use. In the `Identifier` field you can use the drop-down list to select the column to use for this purpose or leave it as `Row Number`.

If you do choose to select a column, you should ensure that this column meets the following requirements:

  1. There must be a value for this column on every row in the CSV file.
  1. The values on each row should be unique.
  1. The values should be a natural identifier for the thing described by the other columns in the row.
  
For more information, read the [Selecting an identifier](/user-guide/choosing-a-license.html) documentation.
  
### Choose visibility 

Before you upload your data, select whether you want your dataset to appear on the DataDock homepage and search results. By default, each dataset is visible on the homepage and search.
	
### Upload the CSV

When you are happy with the metadata, keywords and datatypes, click on the `Publish Data` button. This will start the upload process that
sends the CSV file and your metadata and conversion settings to the DataDock server. Once the files are received, you will be taken to the
`Job History` page which will display the new import job at the top of the page. Once the job starts processing, log messages will appear on this
screen. Once the job is completed, the complete log is available to download as a text file using the link displayed on the Job History page.

If errors are encountered during the processing, the job log entry will turn red. You should review the log messages for any ERROR messages. It may be 
possible to correct errors either by cleaning up or reformatting your input CSV file, or by changing the datatypes you selected at the import stage. If
this is the case you should retry with the updated CSV or with different configuration settings. However if the errors persist or you are unsure what the
error messages mean you should [get in touch with us](./getting-help.html) and we will do our best to help.

### Explore Your Data

If the conversion process completes successfully, at the end of the process your data is published and ready to be explorerd. You can do this by returning
to your Dashboard page where you should see the new dataset shown at the top of the dataset list. Click on the `Explore` button to go to the dataset metadata
page from where you can start to explore some of the data in the dataset.

[&lArr; Back to User Guide](/user-guide/)


