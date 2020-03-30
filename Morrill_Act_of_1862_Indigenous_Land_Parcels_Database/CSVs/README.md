# CSV files #
Here's a rundown of files in this directory. For more information, see/download the pdf [User Guide](https://github.com/HCNData/landgrabu-data/blob/master/Morrill_Act_of_1862_Indigenous_Land_Parcels_Database/LandGrabU_HCN_April_2020.pdf).

### 1. Parcels.csv ###
This file contains data on 79,461 land parcels redistributed through the Morrill Act (or in lieu thereof) across 43 columns. Each row described the location of a unique parcel, along with information about the tract, its original Indigenous owners, its acquisition by the United States, and its benefit to one or more land-grant universities. It also contains source material on how the parcel was identified and retrieved, and material on how—and how accurately—it was mapped.
The data can be mapped by joining the file to **"Parcel_Polygons.shp"** using the field named **MTRSA_LG**.


### 2. Cessions.csv ### 
This file contains data on 162 Indigenous land cessions across 15 columns. Each row describes a unique Indigenous land cession that overlaps with one or more Morrill Act parcels (except for one row for “unknown”). The main source for the land cessions is the set of maps drawn by Charles Royce in the late nineteenth century. The rows provide information about the cession, including the Royce schedule identification number, the name or names of the tribal nations who made the cession, the date and manner of cession, the size of the cession in acres, and payments made by the United States for Indigenous title (if any). It also contains source material on the cession. Since the sheet is constructed around the cessions themselves, multiple tribes may be associated with one record. To find individual tribal nations, use the search function to “filter” the Tribal_Nation column. Use the same technique on the Cession_State column (filtering by state postal code) to identify records mentioning specific states where the cessions were located.

Note that the cessions identified as overlapping the Morrill Act parcels are restricted to initial acquisitions of title by the United States. There are certainly some parcels in this dataset that overlap with reservations of nations removed to the West that were created, then retaken, by the United States, but those cessions do not appear in this dataset.

The data can be mapped by joining the file to **“Cession_Polygons.shp”** using the field named **Royce_Num**.

### 3. Universities.csv ### 
This file contains data on 52 land-grant universities across 54 columns. Each row described a unique university (except for one row for “unknown”) that benefited from a land-grant endowment made under the Morrill Act (or in lieu thereof), along with information about the university’s location, founding and assignment of the grant, what type of grant was received, whether the institutions are public or private, if the benefit was shared by multiple institutions, and the financial interest derived from the grant in terms of endowment principal raised by the early twentieth century and the value of unsold land at that time. There is also source material on how the material was collected and analyzed. To find a succinct text explaining how each state disposed of their grant, see the ‘Disposal Notes’ column, which is summarized primarily from Benjamin F. Andrews, “The Land Grant of 1862 and the Land-Grant Colleges” (1918).

The data can be mapped by joining the file to **“Universities_Points.shp”** using the field named **University**.
