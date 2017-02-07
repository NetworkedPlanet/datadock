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
	 
  1. **DO** ensure that the data you are publishing is either data that you own or data tha has been published under a license that allows
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
     CSV in UTF-8 format.
   
## Sign Up for GitHub

If you have already signed up and configured a GitHub repository for your account, you can skip on to Import Your Data.

To use DataDock you will need a GitHub user account and a public repository that the user account has full read/write access to.
If you do not yet have a GitHub account, you can [sign-up for GitHub here](https://github.com/join/).

## Create a Repository

Your DataDock data is all stored within a GitHub repository that you own - this gives you complete control over your data at all times.
We strongly recommend that you create a repository specifically for use with DataDock. Please ensure that this repository is created as a Public repository.

**IMPORTANT**: When creating a new GitHub repository please ensure that the repository is created with some content on the default branch. The
simplest way to do this, is to check the `Initialize this repository with a README` checkbox when creating the repository through the GitHub site
or from the GitHub client application.

## Sign Up for DataDock

You use your GitHub account credentials to sign up for DataDock. When you click on the Sign Up link you will be asked to log in to your GitHub account (if 
you are not already logged in) and then grant the DataDock application access to your account. We use this access to create and update data in the repository
you choose. After the granting access to the application, you will finally be asked to confirm that you agree to our 
[Terms of Service](http://manage.datadock.io/terms).

## Configure Your Account Settings

This step only needs to be done once when you sign up a new account.

On the [account settings](http://manage.datadock.io/settings) page, first choose the repository you want to use to store your data. As mentioned above,
we strongly recommend you use a separate GitHub repository for your DataDock datasets. The drop-down list shows all of the Public repositories
that you have write access to. If necessary you can create a new repository on GitHub and then return to this page (and refresh the page) to select the newly
created repository.

You should give your repository a title and description - these are separate from the name and description on GitHub and are used in the metadata published for
your data repository.

You should select a default language and timezone. At the moment, the value you choose here is not used, but we plan in future to use these to improve the 
detection of and generation of date/time values as well as to output multi-lingual data.

Finally you may complete any or all of the fields of publisher information, choosing whether you publish as an individual or on behalf of an organisation. 
Please be aware that this information will be public and will be included in the metadata for each dataset you publish.

Once you are happy with these settings, click the Save button to update them.
 
## Import Your Data

Go to your [dashboard](http://manage.datadock.io/sashboard) page and click [Add Data](http://manage.datadock.io/import) to load your data. 
You will be required to select the file containing the CSV data you wish to import. That data will first be loaded locally so that you can
review it and configure how it will be processed into Linked Data.

First, update the title of the dataset (it will default to the name of the file you selected); add a description and select a license. 
We recommend using the CC-0 for friction-free open data). You may also want to tag your data with one or more tags that can help other users to find it.

The import process will attempt to determine the correct datatype for each column in your data. You should check the columns listed
to ensure that all the columns in your data are listed and that the correct datatype has been selected. If necessary you can 
change the column datatypes using the drop-down lists.

When you are satisfied that everything is described correctly, click on the "Start Import" button. This will upload your CSV data
and the configuration information to DataDock for processing. Once the data upload is complete your browser will take you to the 
jobs page where you can monitor the progress of your conversion job. Jobs are queued and processed in order by a batch processing system so at times
of heavy load there may be a wait for a worker to become available. Once your job starts, progress messages will be displayed on the jobs page.

When your job has completed processing, return to the dashboard for your account and you will see your new dataset listed there. You can use
the Explore link to visit the HTML pages that have been generated from your data. Congratulations you are now a publisher of Linked Open Data!
