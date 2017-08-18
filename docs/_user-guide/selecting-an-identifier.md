---
title: Selecting An Identifier
layout: page
order: 110
---

During the DataDock conversion process, each record in your spreadsheet is turned into an entity ready for use on the Web of Data. As everything on the Web of Data has an address, DataDock produces an **identifier** using the row number of the record. If you wish to use a different column for use in the identifier, you can set this during the upload process.

## Example

The default identifier uses the row number such as:
 `http://datadock.io/GitHubUser/DemoRepository/id/resource/companies.csv/row_1`
 
If you have a column full of values that you would like to be used in the identifier instead of the row number, then select it from the drop down list in the settings panel. 
  
 If the companies.csv spreadsheet in the example above has a "Company ID" column, selecting it would produces identifiers such as:
  
 `http://datadock.io/GitHubUser/DemoRepository/id/resource/company_id/1`
 
## Selecting an identifier
 
 After you have selected a file for import, the identifier can be set on the "Advanced" tab. The drop down list shows all columns from your data that could be used as the identifier. 
 
 The values from the column you choose for an identifier do not have to be numerical, but they **must be unique to that dataset**. It's also important that there are **no empty values** in the column you have selected to be in your identifiers. 
 
## Important Note
 
 As you can see from the example above, if you select a column to be used in your identifiers, the name of the dataset is removed from the identifier. This allows you to upload multiple spreadsheets about the same subjects and specify that the data relates to the same subject by selecting the same identifier.
 
 This means you must be careful if selecting a generic identifier such as "ID", as you may well use that same identifier with an import of data that is about different subjects.
 
 Future features of DataDock will include the ability to upload to multiple repositories, and also allow advanced editing of the identifier. For now, make sure that your ID columns are **well named** for clarity.
 
 [&lArr; Back to User Guide](/user-guide/)
