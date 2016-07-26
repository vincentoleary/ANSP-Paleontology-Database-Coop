#Paleontology Database Documentation

Repository for ANSP Vertebrate Paleontology database. Intended for use by lab volunteers and co-op students entering data for Vertebrate Paleontology. 

> This table describes all the fields currently used in the database. It is a reference for entering data correctly and using the correct vocabulary or structure each fields requires. Controlled vocabulary is very important to make sure that records are acurrate and can be used for other programs. Data should be entered as complete as possible for every field.

> The first column 'FileMaker' is the name of the column in FileMaker. They are shown here in the order found in FileMaker.

> The second column 'Darwin Core Field' is the name of the matching fields used by the Darwin Core standards (http://rs.tdwg.org/dwc/terms/index.htm). This is important when the data is added to external projects like iDigBio (https://www.idigbio.org/) or larger databases within the Academy.

> The third column 'Definition' describes the use of that column and what data should be entered into the field. This may seem obvious for something like Catalog Number, but can be confusing when trying to differentiate between identification notes and taxon notes. Whenever in doubt about where to add new data, consult the definitions of each field and choose appropriately.

> The fourth and final column 'Example' provides examples of expected data for that field and how it should be written. For fields such as Collector, where the data can invole multiple people and initials, it is very important to follow the rules and enter the data as described here. When this data is exported for other projects it expects the data to be written correctly and can result in errors if it is not. Some fields may ask for the same information twice and it is useful to look at the examples to understand what is needed in each field. For example, Coordinates should contain the Latitude and Longitude written in a specific way, while Latitude and Longitude should only be written as decimal degrees if known.

------

| FileMaker Field | Corresponding Darwin Core Field | Definition | Example |
|---|---|---|---|
| catalog ID ||A unique identifier for the Record (auotmatically generated)||
| catalog # ||An identifier for the Record within the data set or collection||
| element ||The combination of all morphological terms for the Record||
| count ||The number of individuals represented present in the Record||
| type status ||Nomenclatural types (type status, typified scientific name, publication) applied to the Record||
| higher taxa ||A list of taxa/clade ranks superior to order. Do not use punctuation to separate terms. If the identification is uncertain, use term "cf." to describe a similar Taxon. Write 'Indet.' if the Taxon is indeterminable||
| order (suborder) ||The full scientific name of the order in which the Taxon is classified. Suborder can be listed in paranthesis () if known. If the identification is uncertain, use term "cf." to describe a similar Taxon. Write 'Indet.' if the Taxon is indeterminable||
| family (subfamily) ||The full scientific name of the family in which the Taxon is classified. Subfamily can be listed in paranthesis () if known. If the identification is uncertain, use term "cf." to describe a similar Taxon. Write 'Indet.' if the Taxon is indeterminable ||
| genus (subgenus) species ||The full scientific name of the genus, (subgenus) and species in which the Taxon is classified. If the identification is uncertain, use term "cf." to describe a similar Taxon. Write 'Indet.' if the Taxon is indeterminable||
| taxon notes ||Comments or notes about the taxon or name||
| identification by ||A list of names of people or groups who assigned the Taxon to the Record. This is followed by the year (if known) in parantheses on which the Record was identified as representing the Taxon||
| identification notes ||Comments or notes about the Identification||
| preparation notes ||A list of preparators and preservation methods for the Record||
| coordinates ||The spatial coordinates of the Location in degrees, minutes, seconds. Written as DD°MM'SS" N, DD°MM'SS" E OR DD°MM.MM' N, DD°MM.MM' E||
| decimmal latitude ||The geographic latitude (in decimal degrees, using the spatial reference system given in datum field) of the geographic center of a Location. Legal values lie between -90 and 90, inclusive||
| decimal longitude ||The geographic longitude (in decimal degrees, using the spatial reference system given in datum field) of the geographic center of a Location. Legal values lie between -180 and 180, inclusive||
| datum ||The ellipsoid, geodetic datum, or spatial reference system (SRS) upon which the geographic coordinates are based||
| georeferenced by ||A list of names of people or groups who determined the georeference (longitude and latitude) for the Record. This is followed by the year (if known) in parantheses on which the Record was georeferenced||
| georeference notes ||Notes or comments about the spatial description determination||
| field # ||An identifier given to the Event in the field||
| field notes ||One of a) an indicator of the existence of, b) a reference to (publication, URI), or c) the text of notes taken in the field about the Event||
| collectors ||A list of names of people or groups who collected the original Record||
| date collected ||The date when the Record was collected, written as Month, Day, Year or MM/DD/YYYY. (Month must be written first)||
| country ||The name of the country or major unit in which the Location occurs||
| state ||The name of the state or province unit in which the Location occurs||
| county ||The name of the county or parish unit in which the Location occurs||
| locality name ||The specific description of the Location||
| location notes ||Comments or notes about the Location, related to a specific region||
| event notes ||Comments or notes about the Event, related to the collection process or some other event in time||
| occurrence notes ||Comments or notes about the Occurrence, related to how the catalogued item was collected or observations from the field about the Record||
| geologic age ||The full name of the geochronologic age or chronostratigraphic stage attributable to the stratigraphic horizon from which the cataloged item was collected||
| lithologic notes ||The combination of all litho-stratigraphic names for the rock from which the cataloged item was collected||
| collection ||The name identifying the project or donation from which the Record was derived||
| disposition ||The current state of a Record with respect to the collection at ANSP||
| media ||A list of of identifiers (publication, global unique identifier, URI) of media associated with the Record||
| references ||A list of identifiers (publication, bibliographic reference, global unique identifier, URI) of literature associated with the Record||
| citation ||A bibliographic reference for the resource as a statement indicating how this record should be cited (attributed) when used (auotmatically generated)||
| withhold ||Reason for witholding data from publication, ie. for privacy concerns||
| created ||The date when the Record was created (auotmatically generated)||
| created by ||The user account which created the Record (auotmatically generated)||
| modified ||The most recent date on which the Record was changed (auotmatically generated)||
| modified by ||The most recent user account which changed the Record (auotmatically generated)||
| other information ||Any other information that is not captured in other fields for the Record (auotmatically generated)||