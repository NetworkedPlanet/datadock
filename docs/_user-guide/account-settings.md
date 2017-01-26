---
title: Account Settings
layout: page
order: 2
---

This document provides a detailed description of the account settings form.

## Target Respository

This field sets the GitHub repository that will be used by the Linked Data Laboratory for storing your datasets as you create them.
The drop-down list shows all Public GitHub repositories that you have at least write access to. This list may include repositories
that are owned by other GitHub users or organisations. To distinguish them each repository in the list shows the name of the user 
in brackets after the repository name. e.g. "datarepo (bob)" indicates a repository named `datarepo` that is owned by the GitHub user `bob`.

We strongly recommend that you create a dedicated new Public repository for the Linked Data Laboratory to use, to ensure that changes made by lodlab
do not get overwritten by other applications. 

Although you can change this setting after importing data into a repository, we recommend that you do not alter it. By altering the setting you 
effectively disconnect the previous repository from the Linked Data Laboratory so it will never get updated, even if you upload updated versions
of existing datasets in that repository.

To recap: We recommend that you (1) create a new public repository for the Linked Data Laboratory to use and (2) do not change this setting once you 
have uploaded your first dataset.

## Title and Description

These text fields allow you to provide a user-friendly title and description for your repository. You may want to use these fields to clearly communicate
what sort of data will be published in your repository. The values in these fields appear in the Linekd Data Laboratory lists of repositories and in the 
metadata files generated for your datasets.

## Default Language

From this drop-down list you can select the default language for your repository. Although this setting is not currently used, we plan to use it as the
default language for any text fields in the data you import and also for the title and description you provided for your repository and for each dataset
when you import it.

## Default Timezone

From this drop-down list you can select the default timezone for your repository. This setting is currently not used. However we plan to us it to provide
a default timezone for any date/time fields in the data you import.

## Data Publisher Info

The following fields are all optional. They are included in the metadata published with each dataset you create in the Linked Data Laboratory. 

**Please be aware that the email and website address you provide will be made public.**

## Delete Account

The `Delete Account` link at the bottom of the page will take you through the process of deleting your Lodlab account and all related information from
the Lodlab portal. For more information please see [Deleting Your Account](./deleting-your-account.html).