# landgrabu-data
Source data for the HCN investigation, "Land-Grab Universities"

### I. Overview ###

This repository contains the “Morrill Act of 1862 Indigenous Land Parcels Database.”

The database is the result of a High Country News investigation that has located more than 99% of all acres distributed through the Morrill Act of 1862 (or in lieu thereof), identified their original, Indigenous inhabitants and care-takers, and researched the principal raised from their sale in the late 19th and early 20th centuries. The database reconstructs approximately 10.7 million acres taken from nearly 250 tribes, bands, and communities through over 160 violence- backed land cessions.

This unique database was created through research into primary source materials including land patent records, congressional documents, historical bulletins, archival and print resources at the National Archives, state repositories, and special collections at universities, digitized historical maps and more. Information for the database was extracted programmatically where possible, primarily from the Bureau of Land Management’s [General Land Office Database](https://glorecords.blm.gov/reference/default.aspx), but in some cases it was transcribed manually from print records, microfilm and microfiche reproductions, or poor quality digital images.

For a full discussion of the project methodology, scope and sources, see the separate essay and source list: [“Methodology: Land-Grab Universities.”](https://www.hcn.org/articles/indigenous-affairs-education-how-we-investigated-the-land-grant-university-system) For a bibliographic background on the study of land-grant universities, especially their ties to Indigenous dispossession, see the separate essay and bibliography: [“Further Reading: Land-Grab Universities.”](https://www.hcn.org/articles/further-reading-on-hcns-land-grants-university-investigation) For the article produced from this database, which gives a sense of how this data set can be deployed for research, see Robert Lee and Tristan Ahtone, [“Land-Grab Universities,”](https://www.hcn.org/issues/52.4/indigenous-affairs-education-land-grab-universities) *High Country News*, April 2020.

### II. Use of the Database ###
The database contained CSV and shapefiles, as well as a multi-tab spreadsheet that aggregates/summarizes key data points. No coding skills are necessary to work with this dataset, but a basic working knowledge of tabular data files and/or GIS is necessary.

The data in the CSV files can be analyzed alone or linked to shapefiles for mapping and analysis with GIS software (e.g. ArcGIS Desktop). The files are organized so users can join the data following the model used by IPUMS-NHGIS for making historical census data publicly available. For basic instructions on joining shapefiles to tabular data in a ArcGIS, see the NHGIS user’s guide. This video tutorial on joining census data (i.e. tabular data) to a GIS file (i.e. a shapefile) walks new users through the process. The join fields are noted in the data descriptions below. Given the size of the parcel data users may find it preferable to import the data into a file geodatabase if working with ArcGIS (the program the shapefiles were created with).

We encourage exploration and use of the database for research, teaching, publication, and other public uses. We also invite feedback if you see omissions, errors or miscalculations. Since no other database of its kind exists—location and financial analysis linked to approximately 80,000 individual land parcels distributed through a Civil War-era law—we are committed to making it publicly available and as robust as possible.

The database administrator can be contacted at: **landgrabu@hcn.org**


### III. Creative Commons License ###
The database is licensed under the *Open Database License* [https://opendatacommons.org/licenses/odbl/1.0/](https://opendatacommons.org/licenses/odbl/1.0/), and the contents under the Creative Commons Attribution-ShareAlike license [https://creativecommons.org/licenses/by-sa/3.0/](https://creativecommons.org/licenses/by-sa/3.0/).
  
  
### IV. Citation
If you re-publish this data or otherwise draw on it as a source for publication, in part or whole, cite as:

Robert Lee, “Morrill Act of 1862 Indigenous Land Parcels Database,” *High Country News*, March 2020.


### V. Files Descriptions ###

The database is comprised of 7 files: 3 [shapefiles](https://github.com/HCNData/landgrabu-data/tree/master/Morrill_Act_of_1862_Indigenous_Land_Parcels_Database/Shapefiles), 3 [CSV files](https://github.com/HCNData/landgrabu-data/tree/master/Morrill_Act_of_1862_Indigenous_Land_Parcels_Database/CSVs), and 1 [excel spreadsheet](https://github.com/HCNData/landgrabu-data/blob/master/Morrill_Act_of_1862_Indigenous_Land_Parcels_Database/Summaries_Uni_State_Treaty_Tribe.xlsx) with 4 internal tabs. 

Descriptions of the contents of the following files appear below. Further readme's with specific instructions can be found in the sub-directories, or you can down the [User Guide](https://github.com/HCNData/landgrabu-data/blob/master/Morrill_Act_of_1862_Indigenous_Land_Parcels_Database/User%20Guide_March_2020.pdf) as a PDF.

#### [Shapefiles](https://github.com/HCNData/landgrabu-data/tree/master/Morrill_Act_of_1862_Indigenous_Land_Parcels_Database/Shapefiles)
1. Parcels_Polygons.shp
2. Cessions_Polygons.shp 
3. Universities_Points.shp

#### [CSV files](https://github.com/HCNData/landgrabu-data/tree/master/Morrill_Act_of_1862_Indigenous_Land_Parcels_Database/CSVs)
4. Parcels.csv
5. Cessions.csv
6. Universities.csv

#### Excel file
[7. Summaries_Uni_State_Treaty_Tribe.xlsx](https://github.com/HCNData/landgrabu-data/blob/master/Morrill_Act_of_1862_Indigenous_Land_Parcels_Database/Summaries_Uni_State_Treaty_Tribe.xlsx)

