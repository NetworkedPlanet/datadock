---
title: Deleting Data
layout: page
order: 5
---

## How To Delete A Dataset

To delete a specific dataset from your repository go to your [Dashboard Page](http://manage.lodlab.com/Dashboard), or to your 
[Dataset List Page](http://manage.lodlab.com/Datasets) and find the entry for the dataset you want to delete and then click on
the `Delete` button next to that dataset. You will be taken to a page where you will be asked to confirm that you really do
want to delete this dataset. If so, click on the `Confirm Deletion` button. 

When you confirm deletion, this will create a new update job to remove the dataset from your repository. Like the import 
jobs, a deletion job is queued and run as a batch process which means that at times of heavy use their may be a delay
while waiting for a worker process to become available. 

The progress of the deletion is reported on the [Conversion History](http://manage.lodlab.com/Jobs) page.

## What Is Deleted

When you delete a dataset, the follwing things happen:

  - All of the data contained in that dataset is removed from your repository.
  - The metadata for the dataset is removed from your repository and from the lodlab search engine. 
  - All of the static RDF and HTML files in your repository are regenerated to remove any data from the deleted dataset.
  - The CSV file and CSV metadata JSON file for the dataset are removed from your GitHub repository.
  
## What Is Not Deleted

We do not currently delete the GitHub releases that were made for this dataset. If you wish, you can manually delete these
releases through the GitHub user interface.