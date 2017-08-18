---
layout: default
title: Getting Started
---

# Getting Started

This section will get you started with the DataDock.

We will show you how to create a free data portal from CSV and have it published to the
world in just 10 minutes.

## Choose Your Data

The first thing to decide on is what you want to publish. Here are a few guidelines 
for making that selection.

  1. **DO NOT** publish any data that could be used to personally identify or otherwise compromise the privacy of other individuals.
     This includes things such as home address information, social security numbers, and email addresses. Ideally
     if you are publishing data about people, the data you publish should be aggregated sufficiently to avoid inadvertently identifying
     individuals; failing that the data must be properly pseudonymised.
	 
  1. **DO** ensure that the data you are publishing is either data that you own or data that has been published under a license that allows
     its republication.
	 
  1. **DO NOT** publish any copyright-infringing material.
      
## Prepare the Data

  1. Ensure that the data is in a single, simple table. This may mean removing comment lines, footnotes, keys and other additional material
     from a spreadsheet. You should ensure that all that remains is the data to be imported and a single header row.
	 
  1. Structure the data so that each row in the table relates to one thing and one thing only. This makes the mapping into 
     the linked data structures much more natural.
	 
  1. Ensure that your data has a single header row and that you use column names in a consistent manner. 
     Only the first row in the data will be processed as a header row and the column names provided in that row will be mapped to linked 
	 data properties. For consistency across all your datasets you should ensure that you use column names in a consistent manner. For
     example, don't use "Location" in one spreadsheet and "Place" in another if both are really the same "Location" property.
	 
  1. Save the cleaned up data as CSV. Ensure that you use commas (,) as the separator and not some other character. Please also save your
     CSV in UTF-8 format. There is a 40 character limit on the length of the file name, and files are limited to a maximum 4MB in size.
   
## Sign Up for GitHub

If you have already signed up and configured a GitHub repository for your account, you can skip on to Import Your Data.

To use DataDock you will need a GitHub user account and at least one public repository that the user account has full read/write access to.
If you do not yet have a GitHub account, you can [sign-up for GitHub here](https://github.com/join/).

## Create a Repository

Your DataDock data is all stored in public GitHub repositories that you have write access to - this gives you complete control over your data at all times.

We strongly recommend that you create repositories specifically for DataDock data, rather than mixing the use of the GitHub repository with other storage.

## Sign Up for DataDock

You use your GitHub account credentials to sign up for DataDock. When you click on the Sign Up link you will be asked to log in to your GitHub account (if 
you are not already logged in) and then grant the DataDock application access to your account. We use this access to create and update data in your target repositories. After the granting access to the application, you will finally be asked to confirm that you agree to our 
[Terms of Service](http://manage.datadock.io/terms).

## Your dashboard

You can access your dashboard at anytime either by navigating to [/dashboard](http://manage.datadock.io/dashboard) directly or using the menu in at the top of the page.

The dashboard menu shows a summary for your GitHub account, the GitHub organisations that you have access to, and an "Everything" level that shows all DataDock data published to both your own GitHub and your organisations.
 
## Import Your Data

Go to [Add Data](http://manage.datadock.io/import) to load your data. 
You will be required to select the file containing the CSV data you wish to import. That data will first be loaded  so that you can review it and configure how it will be processed before publishing.

### Dataset Details

First, update the title of the dataset (it will default to the name of the file you selected); add a description and select a license. 
We recommend using the CC-0 for friction-free open data). You may also want to tag your data with one or more tags that can help other users to find it.

### Column Definitions

The import process will attempt to determine the correct datatype for each column in your data. You should check the columns listed
to ensure that all the columns in your data are listed and that the correct datatype has been selected. If necessary you can 
change the column datatypes using the drop-down lists.

### Advanced 

If you are comfortable with Linked Data, you can selected a specific column to be used in each record's identifier, and also customise the property URLs (also known as predicates) used. 

For those new to Linked Data, it is recommended to leave the default values in place.

When you are satisfied that everything is described correctly, choose whether you wish the dataset to be visible on the DataDock homepage and search results. Then click on the "**Publish**" button. 

This will upload your CSV data
and the configuration information to DataDock for processing. Once the data upload is complete your browser will take you to the 
jobs page where you can monitor the progress of your conversion job. Jobs are queued and processed in order by a batch processing system so at times
of heavy load there may be a wait for a worker to become available. Once your job starts, progress messages will be displayed on the jobs page.

When your job has completed processing, return to the dashboard for your account and you will see your new dataset listed there. You can use
the Explore link to visit the HTML pages that have been generated from your data. Congratulations you are now a publisher of Linked Open Data!
