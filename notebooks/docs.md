# LandMark

[LandMark documentation](https://communityland.s3.amazonaws.com/LandMark_public/LandMark_Data_Quality_v202408.pdf)

| Col | Description | dtype |
|-----|-------------|-------|
| `identity` | How does the community self-identify? As Indigenous Peoples or as non-indigenous local community? *When unclear or unknown, the land is presented as community land.* | `chr` |
| `name` | What is the name of the selected indigenous or community land? | `chr` |
| `form_rec` | Is the indigenous or community land formally recognized by law or decree (e.g. recognized as the property or as lawfully occupied and used by Indigenous Peoples and/or local communities)? Presented as “Acknowledged by government” or “Not acknowledged by government” or “Unknown” for Indicative lands | `chr` |
| `doc_status` | What is the documentation status of the land (e.g. the stage of lawful ownership or occupation endowment process)? (Documented, Not documented, Held or used with formal land claim submitted, Held or used under customary tenure (without formal land claim submitted)) | `chr` |
| `stat_date` | The year that the land attained the specified documentation status (if known). | `chr` |
| `stat_note` | (Not mentioned in documentation) Specific information such as name of act/resolution | `chr` | 
| `country` | In what country is the indigenous/community land located? | `chr` |
| `category` | What is the categorical name that the local state gives to this type of indigenous or community land? (e.g. indigenous territories, tribal lands, village lands, communal lands, customary lands). | `chr` |
| `ethncty_1` | What are the names of the principal ethnic groups that reside on the indigenous or community land? | `chr` |
| `populatn` | How many people normally reside on the indigenous or community land? | `num` |
| `pop_source` | Source of population estimate/census | `chr` |
| `pop_year` | Year of population estimate/census | `num` |
| `area_ofcl` | What is the official area of the indigenous or community land, as stated in the formal documents (only applies to formally recognized lands)? (hectares) | `num` |
| `area_gis` | What is the area of the land as calculated in GIS? (hectares) If the community land is not officially mapped or with GIS information, please indicate the estimated size of the area, followed by (est.). | `num` |
| `scale` | What is the scale at which the land data were collected or georeferenced? | `chr` |
| `method` | What was the method used to acquire the indigenous or community land data (e.g., hand-held GPS, transcribed from land title)? | `chr` |
| `data_ctrb` | Which individual or organization provided the data to LandMark? | `chr` |
| `data_src` | Which individual or organization created the data that are shown on LandMark? May or may not be the same as the contributing institution. | `chr` |
| `data_src_s` | Presumably "short", source acronym | `chr` |
| `data_src_l` | Presumalby "long", full name of source | `chr` |
| `data_date` | Date that data were created or last edited. | `chr` |
| `add_note` | Additional notes to explain or clarify any information provided about the indigenous or community land. | `chr` |
| `more_info` | A web link to more detailed information. | `chr` |
| `layer` | Type - "Indigenous Lands"/"Community Lands" | `chr` |
| `download` | Presumably whether it was downloaded (all "Yes") | `chr` |
| `iso_code` | Country ISO code | `chr` |
| `geometry` | Multipolygon of area | `sfc_MULTIPOLYGON of length 124616` |

# Interagency Fire Perimeter History

[IFPH Documentation](https://data-nifc.opendata.arcgis.com/datasets/nifc::interagencyfireperimeterhistory-all-years-view/about)

| Col | Description | dtype |
|-----|-------------|-------|
| `IRWINID` | Primary key for linking to the IRWIN Incident dataset. The origin of this GUID is the wildland fire locations point data layer maintained by IrWIN. (This unique identifier may NOT replace the GeometryID core attribute) | `chr` |
| `FORID` | Unique identifier assigned to each incident record in the Fire Occurence Data Records system. (This unique identifier may NOT replace the GeometryID core attribute) | `chr` |
| `INCIDENT` | The name assigned to an incident; assigned by responsible land management unit. (IRWIN required). Officially recorded name. | `chr` |
| `GIS_ACRES` | GIS calculated acres within the fire perimeter. Not adjusted for unburned areas within the fire perimeter. Total should include 1 decimal place. (ArcGIS: Precision=10; Scale=1). Example: 23.9 | `num` |
| `UNQE_FIRE` | Unique fire identifier is the Year-Unit Identifier-Local Incident Identifier (yyyy-SSXXX-xxxxxx). SS = State Code or International Code, XXX or XXXX = A code assigned to an organizational unit, xxxxx = Alphanumeric with hyphens or periods. The unit identifier portion corresponds to the POINT OF ORIGIN RESPONSIBLE AGENCY UNIT IDENTIFIER (POOResonsibleUnit) from the responsible unit’s corresponding fire report. Example: 2013-CORMP-000001 | `chr` |
| `DATE_CUR` | The last edit, update, or other valid date of this GIS Record. Example: mm/dd/yyyy. | `chr` |
| `FIRE_YEAR_` | Integer version of `FIRE_YEAR` | `int` |
| `UNIT_ID` | NWCG Unit Identifier of landowner/jurisdictional agency unit at the point of origin of a fire. (NFIRS ID should be used only when no NWCG Unit Identifier exists). Example: CORMP | `chr` |
| `POO_RESP_I` | ? | `chr` |
| `LOCAL_NUM` | Local incident identifier (dispatch number). A number or code that uniquely identifies an incident for a particular local fire management organization within a particular calendar year. Field is string to allow for leading zeros when the local incident identifier is less than 6 characters. (IRWIN required). Example: 123456. | `chr` |
| `FEATURE_CA` | Type of wildland fire polygon: Wildfire (represents final fire perimeter or last daily fire perimeter available) or Prescribed Fire or Unknown | `chr` |
| `MAP_METHOD` | Controlled vocabulary to define how the geospatial feature was derived. Map method may help define data quality. (GPS-Driven; GPS-Flight; GPS-Walked; GPS-Walked/Driven; GPS-Unknown Travel Method; Hand Sketch; Digitized-Image; Digitized-Topo; Digitized-Other; Image Interpretation; Infrared Image; Modeled; Mixed Methods; Remote Sensing Derived; Survey/GCDB/Cadastral; Vector; Other) | `chr` |
| `COMMENTS` | Additional information describing the feature. Free Text. | `chr` |
| `GEO_ID` | Primary key for linking geospatial objects with other database systems. Required for every feature. This field may be renamed for each standard to fit the feature. Globally Unique Identifier (GUID). | `chr` |
| `SOURCE` | System/agency source of record from which the perimeter came. | `chr` |
| `AGENCY` | Agency assigned for this fire - should be based on jurisdiction at origin. | `chr` |
| `FIRE_YEAR` | Calendar year in which the fire started. Example: 2013. Value is of type integer (FIRE_YEAR_INT) | `chr` |
| `GlobalID` | Presumably global identifier | `chr` |
| `geometry` | Multipolygon of area | `sfc_MULTIPOLYGON of length 116337` |