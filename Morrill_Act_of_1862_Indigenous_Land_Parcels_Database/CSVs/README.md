# CSV files #
Here's a rundown of files in this directory. For more information, see/download the pdf [User Guide](https://github.com/HCNData/landgrabu-data/blob/master/Morrill_Act_of_1862_Indigenous_Land_Parcels_Database/LandGrabU_HCN_April_2020.pdf).

### 1. Parcels.csv ###
This file contains data on 79,461 land parcels redistributed through the Morrill Act (or in lieu thereof) across 43 columns. Each row described the location of a unique parcel, along with information about the tract, its original Indigenous owners, its acquisition by the United States, and its benefit to one or more land-grant universities. It also contains source material on how the parcel was identified and retrieved, and material on how—and how accurately—it was mapped.
The data can be mapped by joining the file to **Parcel_Polygons.shp** using the field named **MTRSA_LG**.

The file contains the following columns:

- **MTRSA_LG**
This is a unique identifier for the parcel. It stands for “Meridian, Township, Range, Section, Aliquot, Land Grant.” MTRSA describes the parcel location within Public Land Survey System (PLSS). MTRSA stands for “Meridian, Township, Range, Section, Aliquot.” LG is the postal abbreviation of the state granted the parcel for the benefit of a land-grant university. To map the parcel, this field can be joined to a field with the same name in “Morrill_Act_Parcels.shp.”

- **Loc_State**
The postal code of the state where the parcel is located.

- **Loc_County**
The name of the county where the parcel is located. Marked “unidentified” if parcel location not identified.

- **Acres**
The size of the parcel in acres, either listed on patents or state selection lists, or surmised from the aliquot description.

- **LG_State**
The postal code of the state granted the parcel for the benefit of a land-grant university. Marked “unidentified” if state grantee (LG_State) not identified.

- **LG_Reason**
Explanation for the identification of the LG_State. Marked “unidentified” if state grantee (LG_State) not identified.

- **University**
The current university beneficiary or beneficiaries of the endowment generated from the land grant this parcel was contained in. Marked “unidentified” if state grantee (LG_State) not identified.

- **Uni_Ben_History**
The university beneficiary or beneficiaries present and past, including the years of the benefit, and percentage of the benefit (if shared). Marked “unidentified” if state grantee (LG_State) not identified.

- Royce_ID
The ID numbers for the Indian land cession maps. This uniquely identifies the Indigenous land cession, as drawn by Charles Royce, that the parcel lies within. Note that there are 156 of these numbers and 6 non-Royce areas derived from other maps and given IDs like “None_CA” or “LA_Atakapa.” Marked “unidentified” if parcel location not identified.

- **Tribal_Nation**
The name(s) of the tribal nation(s) that ceded the land according to Charles Royce’s schedule of Indian land cessions. Note the names appear as they do on Royce’s schedule from the nineteenth century. Many of the names are no longer in use. Some are considered offensive. Marked “unidentified” if parcel location not identified.

- **US_Acquired_Mode**
Describes the mode by which the US acquired the land, e.g. treaty, unratified treaty, seizure, as well as the date of the action. Marked “unidentified” if parcel location not identified.

- **Cession_State**
The postal code of the modern state or states where the Indigenous land cession that later supplied this parcel was located. Marked “unidentified” if parcel location not identified.

- **Royce_Link**
A link to the web address of the cession listed in Royce’s schedule of Indian land cessions. Marked “unidentified” if parcel location not identified.

- **Yr_US_Acquire**
The year the US acquired the Indigenous land supplying this parcel (format: YYYY). Marked “na” if acquisition year not known. Marked “unidentified” if parcel location not identified.

- **Date_US_Acquire**
The date the US acquired the Indigenous land supplying this parcel (format: YYYYMMDD). Marked “na” if acquisition date not known. Marked “unidentified” if parcel location not identified.
- **US_Paid_for_Parcel**
The amount the United States paid to extinguish Indigenous title. Calculated from the amount paid per acre for the cession (US_Paid_Per_Acre in Cessions.csv) multiplied by the number of acres in the parcel. Marked “unidentified” if parcel location not identified.
- **Endow_Raised_Parcel**
The amount of principal raised for the land-grant endowment plus the value of unsold land ca. 1914 attributable, on average, to the parcel. Based on the total amount of principal raised plus the value of unsold land ca. 1914 per acre in the grant (based on acres found), multiplied by the number of acres in the parcel. Marked “unidentified” if state grantee (LG_State) not identified.
- **Uni_Raise_US_Pay_Multiple
The Endow_Raised_Parcel divided by the US_Paid_for_Parcel. The return on the endowment raised relative to the amount paid by the United States for Indigenous title. For example, if the Uni_Raise_US_Pay_Multiple = 50, then $50 dollars was raised for the endowment for every $1 the U.S. paid for Indigenous title. Where US_Paid_for_Parcel = 0, the multiple is listed as “incalculable.” Marked “unidentified” if parcel location not identified.
- **Yr_ST_Accept**
The year the state accepted the grant (format: YYYY). Marked “unidentified” if state grantee (LG_State) not identified.
- **Yr_Uni_Assign**
The year the state assigned the grant (format: YYYY). Marked “unidentified” if state grantee (LG_State) not identified.
- **Yr_Patent**
The year a land patent was issued for the parcel, if known (format: YYYY).
- **Date_Patent**
The date a land patent was issued for the parcel, if known (format: YYYYMMDD).
- **Patentees**
The name or names of the patentee or patentees who acquired the patent for the parcel.
- **Patent_Source_Reason
Explanation for the assignment of the Yr_Patent / Date_Patent/Patentees.
- **Source_ID**
Identification for the source document. Note that the vast majority of the entries come from the BLM’s General Land Office patent database. When the ID is a number followed by AGS (Agricultural Scrip), SER (Serial Patent), or MV (Miscellaneous Volume) and a state postal code, the preceding number can be used to search for the patent in the BLM database. When the ID is a number preceded by CDI (Control Document Index), the succeeding number can likewise be used to search for the control document index entry in the BLM database. Other IDs, which generally start with a state postal code, followed by a number were created to refer back to transcribed lists of state grant parcels from various other sources, which were integrated into this master parcel list. For these sources, as well as information on their format, and how they were added to this list, see the Source_Loc, Source_Type, Source_Form, and Source_Acqu fields. For links to sources that are available online, see the Parcel_Link field.
- **Source**
Indicates the source for the entry.
- **Source_Loc**
The location of original documentation for the entry.
- **Source_Type**
The format of the original documentation for the entry: Manuscript or Published.
- **Source_Form**
The form of the source for the entry: Archival, Digital, Microfiche, Microfilm, Print.
- **Source_Acqu**
How the entry data was added to the parcel list: Database extraction or Transcribed.
- **Source_Acqu_Detail
Details how the entry data was acquired.
- **Located_GIS**
Indicates if the parcel was mapped in Geographic Information Science software and is represented by a polygon in “Morrill_Act_Parcels.shp”: “Y” for Yes, “N” for No. Note that only 100 parcels, representing about 7,100 acres, could not be mapped.
- **Parcel_Link**
A web address for the source of the parcel. Available for 74,270 parcels (ca. 93%). Most link to the BLM’s General Land Office patent database.
- **MTRSA**
Stands for “Meridian, Township, Range, Section, Aliquot.” MTRSA describes the parcel’s location within the Public Land Survey System.
- **MTRS**
Stands for “Meridian, Township, Range, Section.” MTRS describes the section (typically a square mile, or 640 acres) of the Public Land Survey System where the parcel is located.
- **A_or_L**
Indicates if the parcel is an Aliquot (“A”) part or Lot (“L”) in the Public Land Survey System. Aliquots are rectilinear parts of sections, e.g. the northwest (NW) corner of section 10. Lots are irregularly shaped parcels, often due to being adjacent to bodies of water and are identified by a number.
- **Aliquot**
Indicates the aliquot part, e.g. NW for northwest corner or E1⁄2SW for east half of southwest corner, or the lot number.
- **Types**
Indicates the type of aliquot part, e.g. Q for quarter section if the aliquot is NW or HQ for half-quarter section if the aliquot is E1⁄2SW, or L if it is a lot.
- **GISAcres**
Area of the parcel in acres calculated in GIS using the US National Atlas Equal Area projection.
- **GIS_Acre_Div_List_Acre**
The ratio of the area of the polygon measured in GIS to the acres for the parcel listed in other documentation, i.e. GISAcres divided by Acres. A useful measure of polygon accuracy.
- **Polygon**
Describes how the polygon was reconstructed.
- **Accuracy**
Describes the accuracy of the polygon reconstructed in GIS. “Aliquot” indicates the highest level of accuracy. It means the polygon is accurate to the aliquot part described in PLSS notation (i.e. the “A” in MTRSA). This means the parcel is roughly accurate to the acre. “Section” indicates the polygon is accurate to the section described in the PLSS notation (i.e. the “S” in MTRSA). This means the parcel is located somewhere inside the section (typically a square mile, or 640 acres), or part thereof, of the PLSS represented by the polygon. Roughly 97% of parcels, and over 99% of the acres, in the dataset that are mapped are accurate to the “Aliquot,” or acre, level. “None” indicates the parcel has not been mapped.
- **LG_Royce**
Combination of the LG_State (the postal code of the state granted the parcel for the benefit of a land-grant university) and the Royce_ID (the Royce map ID number).


### 2. Cession_Polygons.shp ### 
This shapefile contains 162 unique polygons representing Indigenous land cessions that overlap with one or more of the parcels distributed through the Morrill Act (or acts in lieu thereof). It can be joined to the [Cessions.csv](https://github.com/HCNData/landgrabu-data/blob/master/Morrill_Act_of_1862_Indigenous_Land_Parcels_Database/CSVs/Cessions.csv) using the field named **Royce_Num**.

### 3. University_Points.shp ### 
This shapefile contains 52 unique points representing the location of universities that benefited from the Morrill Act (or acts in lieu thereof). It can be joined to the [Universities.csv](https://github.com/HCNData/landgrabu-data/blob/master/Morrill_Act_of_1862_Indigenous_Land_Parcels_Database/CSVs/Universities.csv) using the field named **Universities**.
