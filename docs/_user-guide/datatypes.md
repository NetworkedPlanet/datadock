---
title: Datatypes
layout: page
order: 100
---

This document describes the different datatypes that are supported by the DataDock conversion process.

## Note On Validation

The current release of the DataDock processing tools do not perform any sort of validation on the content
of cells. We plan to implement such validation at a later date - when this validation is implemented, any cells that
do not meet the validation requirements of the selected datatype for their column will be rejected, resulting in 
a failed conversion process.

## Datatype Descriptions

### Date

Use for columns that contain a date without any time component to it. Currently we do not validate the content of
cells for conformance to a date pattern, however future versions of the tool will validate this conformance and 
will require that dates be expressed either in YYYY-MM-DD format or in the usual format for your chosen default
langugae locale.

In the output RDF data Date columns will result in XML Schema date datatype values.

### Date And Time

Use for columns that contain a date with a time component to it. 

Currently we do not validate the content of
cells for conformance to a date/time pattern, however future versions of the tool will validate this conformance and 
will require that dates be expressed either in YYYY-MM-DD hh:mm:ss format, or in ISO YYYY-MM-DDThh:mm:ss format or in 
the usual format for your chosen default langugae locale.

In the output RDF data these columns will result in XML Schema dateTime datatype values.

### Decimal Number

Use for columns that contain numeric data with an optional decimal part.  Both positive and negative values are supported.

Currently we do not validate the content of cells for conformance to a decimal number pattern. However future versions of the tool will validate this conformance
using the usual numeric separators for your chosen default language locale.

In the output RDF data these columns will result in XML Schema decimal datatype values.

### Text

Use for columns that should be imported as plain text.

In the output RDF data these columns will result in XML Schema string datatype values.

### True / False

Use for columns that should be processed as a boolean true/false value. Currently we do not validate the content
of cells for conformance to a boolean pattern. However future versions of the tool will validate this conformance
and will require that the content be "TRUE", "T" or "1" for true values and "FALSE", "F" or "0"
for false values (using case-insensitve string matching).

In the output RDF data these columns will result in XML Schema boolean datatype values.

### URI

Use for columns that contain URIs or URLs such as links to web pages, or URI identifiers for other linked data resources.

Content will be validated for conformance to the URI specification.

In the output RDF data these columns will result in XML Schema boolean anyURI values.

### Whole Number

Use for columns that contain numeric data with no decimal part. Both positive and negative values are supported.

Content will be validated for conformance using the usual numeric separators for your chosen default language.


[&lArr; Back to User Guide](/user-guide/)
