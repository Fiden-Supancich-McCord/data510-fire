# Data Documentation

This covers the original data format (not including transformations or any cleaning steps).

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

# InFORM Fire Occurrence Data

[InFORM documentation](https://data-nifc.opendata.arcgis.com/datasets/nifc::inform-fire-occurrence-data-records/about)

| Col | Description | dtype |
|-----|-------------|-------|
| `OBJECTID` | | `numeric` |
| `ABCD.Misc` | A FireCode used by USDA FS to track and compile cost information for emergency initial attack fire suppression expenditures. for A, B, C & D size class fires on FS lands. | `chr` |
| `ADS.Permission.State` | Indicates the permission hierarchy that is currently being applied when a system utilizes the UpdateIncident operation. | `chr` |
| `Calculated.Acres` | A measure of acres calculated (i.e., infrared) from a geospatial perimeter of a fire.  More specifically, the number of acres within the current perimeter of a specific, individual incident, including unburned and unburnable islands.  The minimum size must be 0.1. | `numeric` |
| `Containment.Date.Time` | The date and time a wildfire was declared contained. | `chr` |
| `Control.Date.Time` | The date and time a wildfire was declared under control. | `chr` |
| `Created.By.System` | ArcGIS Server Username of system that created the IRWIN Incident record. | `chr` |
| `Created.On.Date.Time` | Date/time that the Incident record was created. | `numeric` |
| `Incident.Size` | Reported for a fire. The minimum size is 0.1. | `numeric` |
| `Discovery.Acres` | An estimate of acres burning upon the discovery of the fire. More specifically when the fire is first reported by the first person that calls in the fire.  The estimate should include number of acres within the current perimeter of a specific, individual incident, including unburned and unburnable islands. | `logical` |
| `Dispatch.Center.ID` | A unique identifier for a dispatch center responsible for supporting the incident. | `char` |
| `Estimated.Cost.To.Date` | The total estimated cost of the incident to date. | `logical` |
| `Final.Acres` | Reported final acreage of incident. | `logical` |
| `Final.Fire.Report.Approved.By.Title` | The title of the person that approved the final fire report for the incident. | `char` |
| `Final.Fire.Report.Approved.By.Unit` | NWCG Unit ID associated with the individual who approved the final report for the incident. | `logical` |
| `Final.Fire.Report.Approved.Date` | The date that the final fire report was approved for the incident. | `char` | 
| `Fire.Behavior.General` | A general category describing the manner in which the fire is currently reacting to the influences of fuel, weather, and topography.  | `logical` |
| `FireCode` | A code used within the interagency wildland fire community to track and compile cost information for emergency fire suppression expenditures for the incident. | `char` |
| `FireDepartmentID` | The U.S. Fire Administration (USFA) has created a national database of Fire Departments.  Most Fire Departments do not have an NWCG Unit ID and so it is the intent of the IRWIN team to create a new field that includes this data element to assist the National Association of State Foresters (NASF) with data collection. | `char` |
| `Fire.Discovery.Date.Time` | The date and time a fire was reported as discovered or confirmed to exist.  May also be the start date for reporting purposes. | `char` |
| `Fire.Mgmt.Complexity` | The highest management level utilized to manage a wildland fire event. | `char` |
| `FireOutDateTime` | The date and time when a fire is declared out. | `char` |
| `FS.Job.Code` | A code use to indicate the Forest Service job accounting code for the incident.  This is specific to the Forest Service.  Usually displayed as 2 char prefix on FireCode. | `char` |
| `FS.Override.Code` | A code use to indicate the Forest Service job accounting code for the incident.  This is specific to the Forest Service.  Usually displayed as 2 char prefix on FireCode. | `char` |
| `GACC` | A code that identifies one of the wildland fire geographic area coordination center at the point of origin for the incident. A geographic area coordination center is a facility that is used for the coordination of agency or jurisdictional resources in support of one or more incidents within a geographic coordination area.| `char` |
| `Incident.Name` | The name assigned to an incident. | `char` |
| `Incident.Short.Description` | General descriptive location of the incident such as the number of miles from an identifiable town. | `logical` |
| `Incident.Type.Category` | The Event Category is a sub-group of the Event Kind code and description. The Event Category further breaks down the Event Kind into more specific event categories. Only WF or RX, presumably for wildfire or prescribed burn. | `char` |
| `Incident.Type.Kind` | A general, high-level code and description of the types of incidents and planned events to which the interagency wildland fire community responds. All FI, presumably fire? | `char` |
| `Initial.Latitude` | The latitude location of the initial reported point of origin specified in decimal degrees. | `numeric` |
| `Initial.Longitude` | The longitude location of the initial reported point of origin specified in decimal degrees. | `numeric` |
| `Initial.Response.Date.Time` | The date/time of the initial response to the incident. More specifically when the IC arrives and performs initial size up. | `char` |
| `Is.Fire.Cause.Investigated` | Indicates if an investigation is underway or was completed to determine the cause of a fire. | `numeric` (bool) |
| `Is.FS.Assisted` | Indicates if the Forest Service provided assistance on an incident outside their jurisdiction. | `logical` |
| `Is.Reimbursable` | | `logical` |
| `Is.Tresspass` | | `logical` |
| `Local.Incident.Identifier` | | `char` |
| ModifiedBySystem | | |
| `Modified.On.Date.Time` | | `char` |
| `Percent.Contained` | | `logical` |
| `City` | | `char` |
| `POO.County` | | `char` |
| `POODispatchCenterID` | | `char` |
| `POO.Fips` | | `numeric` |
| `POO.Jurisdictional.Agency` | | `char` |
| `POO.Jurisdictional.Unit` | | `char` |
| `POO.Jurisdictional.Unit.Parent.Unit` | | `char` |
| `POO.Landowner.Category` | | `char` |
| `POO.Landowner.Kind` | | `char` |
| `POO.Protecting.Agency` | | `char` |
| `POO.Protecting.Unit` | | `char` |
| `POO.State` | | `char` |
| `Predominant.Fuel.Group` | | `char` |
| `Predominant.Fuel.Model` | | `char` |
| `UniqueFireIdentifier` | | `char` |
| `FORID` | | `char` |

Additional variables that were not listed in the documentation: 

- Initial.Response.Agencies
- Fire.Cause
- Fire.Cause.General
- Fire.Cause.Specific
- Fire.Cause.Specific.Detail
- Fire.Cause.Age.Category
- Fire.Cause.Activity.Group
- GlobalID
- IsCauseProhibited
- ModifiedBySystem
- Related.Irwin.IDs
- Status
- AcresBIA
- AcresBLM
- AcresBOR
- AcresDOD
- AcresDOE
- AcresNPS
- AcresUSFS
- AcresUSFWS
- AcresForeign
- AcresTribal
- AcresCity
- AcresCounty
- AcresState
- AcresPrivate
- AcresANCSA
- AcresOtherLocal
- AcresOtherFederal
- Fire.Cause.Comments
- Calendar.Year
- x
- y
