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
