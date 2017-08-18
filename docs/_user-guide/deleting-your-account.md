---
title: Deleting Your Account
layout: page
order: 70
---

## How To Delete Your Account

To delete your account you must first [log in](http://manage.datadock.io/account/login) and then use the user menu drop down (top right) to navigate to your `Account Settings`. 

On the Account Settings page, click on the Delete Account link located at the bottom of the page.
You must check the box to confirm that you wish to delete your account permanently and then click
on the `Delete My Account` button to proceed.

Once your account on DataDock is deleted you may also want to revoke the GitHub access that the application has.
To do this, log in to your GitHub account and go to your [GitHub account settings](https://github.com/settings/applications) page. 
Click on `Authorized Applications` on the left-hand side and find the application named `DataDock Management Portal` and click on the `Revoke` button next to that application.

## What Is Deleted ?

When you delete your DataDock account we remove:

  - Your user settings
  - The search metadata we hold about the datasets in your repository
  - The data conversion history records for your repository
  
This means that

  1. The datasets contained in your repository will no longer appear in search results
     or in dataset lists on the DataDock site.
	 
  1. Should you choose to recreate your account at a later date you will need to re-enter 
     your user settings and any past history about or records of the datasets contained in
	 any of your GitHub repositories will be lost.
	 
## What Is Not Deleted ?

Deleting your user account *DOES NOT* delete your datasets or the static HTML and RDF files that DataDock created for your data. As long as your repository remains public, these files are still accessible to
the public either directly through the GitHub Pages site for your repository, or indirectly through the [datadock.io](http://datadock.io/)
portal.

## To Delete Specific Data

If you want to delete one or more datasets from your repository you can do this without deleting your account. For more information
please refer to [Deleting Data](./deleting-data.html).

[&lArr; Back to User Guide](/user-guide/)
