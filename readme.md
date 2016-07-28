#Darwin Core Standards for Paleontology

Repository for ANSP Vertebrate Paleontology database. Intended for use by lab volunteers and co-op students entering data for Vertebrate Paleontology. This table describes all the fields currently used in the database. It is a reference for entering data correctly and using the correct vocabulary or structure each fields requires. Controlled vocabulary is very important to make sure that records are acurrate and can be used for other programs. Data should be entered as complete as possible for every field. 

Tables are separated into catergories based on Darwin Core. Names that begin with dcterms: are terms managed by the Dublin Core Metadata Initiativem adapted by Darwin Core for biodiversity applications.

When using the ANSP database to enter data, refer to the FileMaker fields and examples. These definitions have been agreed upon to represent all the data recorded in FileMaker. From within FileMaker there is a way to export the data into a new Darwin Core table that converts everything into the format required. This only works when data is entered correctly and as expected into FileMaker.

> The first column 'FileMaker' is the name of the column in FileMaker. Sometimes a term may be used more than once if there are multiple Darwin Core fields being represented, but it will only need to be entered into one column in FileMaker. "N/A" is used when there is a Darwin Core field without a corresponding column in FileMaker or multiple FileMaker field refers to one Darwin Core field.

> The second column 'Darwin Core Field' is the name of the matching fields used by the Darwin Core standards (http://rs.tdwg.org/dwc/terms/index.htm). This is important when the data is added to external projects like iDigBio (https://www.idigbio.org/) or larger databases within the Academy.

> The third column 'Definition' describes the use of that column and what data should be entered into the field. This may seem obvious for something like Catalog Number, but can be confusing when trying to differentiate between identification notes and taxon notes. Whenever in doubt about where to add new data, consult the definitions of each field and choose appropriately.

> The fourth and final column 'Example' provides examples of expected data for that field and how it should be written. For fields such as Collector, where the data can invole multiple people and initials, it is very important to follow the rules and enter the data as described here. When this data is exported for other projects it expects the data to be written correctly and can result in errors if it is not. Some fields may ask for the same information twice and it is useful to look at the examples to understand what is needed in each field. For example, Coordinates should contain the Latitude and Longitude written in a specific way, while Latitude and Longitude should only be written as decimal degrees if known.

> All definitions and examples were drawn from Darwin Core standards (http://rs.tdwg.org/dwc/terms/index.htm) and adapted for the specific needs of the Vertebrate Paleontology collection at the Academy of Natural Sciences.

###Record-Level terms 

|FileMaker Field|Darwin Core Field|Definition|Example|
|---|---|---|---|
|N/A|dcterms:type|The nature or genre of the resource|PhysicalObject|
|created||The date when the Record was created (auotmatically generated)|01/01/2016|
|created by||The user account which created the Record (auotmatically generated)|abc123|
|modified|dcterms:modified|The most recent date on which the Record was changed (auotmatically generated)|01/01/2016|
|modified by||The user account which changed the Record (auotmatically generated)|abc123|
|citation|dcterms:bibliographicCitation|A bibliographic reference for the resource as a statement indicating how this record should be cited (attributed) when used (auotmatically generated)|"Ctenomys sociabilis (MVZ 165861)" for a specimen|
|N/A|institutionCode|The name (or acronym) in use by the institution having custody of the object(s) or information referred to in the record|ANSP|
|N/A|collectionCode|The name, acronym, coden, or initialism identifying the collection or data set from which the record was derived|Vertebrate Paleontology|
|collection|datasetName|The name identifying the project or donation from which the Record was derived||
|N/A|basisOfRecord|The specific nature of the data record|FossilSpecimen|
|withhold|informationWithheld|Reason for witholding data from publication, ie. for privacy or environmental concerns||
|other information||Any other information that is not captured in other fields for the Record (auotmatically generated)||

###Occurrence terms
|FileMaker Field|Darwin Core Field|Definition|Example|
|---|---|---|---|
|catalog ID|occurrenceID|A unique identifier for the Record (auotmatically generated)||
|catalog #|catalogNumber|An identifier for the Record within the data set or collection||
|collectors|recordedBy|A list of names of people or groups who collected the original Record||
|count|individualCount|The number of individuals represented present in the Record||
|preparation notes|preparations|A list of preparators and preservation methods for the Record||
|disposition|disposition|The current state of a Record with respect to the collection at ANSP||
|media|associatedMedia|A list of of identifiers (publication, global unique identifier, URI) of media associated with the Record||
|references|associatedReferences|A list of identifiers (publication, bibliographic reference, global unique identifier, URI) of literature associated with the Record||
|occurrence notes|occurrenceRemarks|Comments or notes about the Occurrence, related to how the catalogued item was collected or observations from the field about the Record||

###Event terms
|FileMaker Field|Darwin Core Field|Definition|Example|
|---|---|---|---|
|field #|fieldNumber|An identifier given to the Event in the field||
|date collected|Year|The date when the Record was collected, written as Month, Day, Year or MM/DD/YYYY. (Month must be written first)||
|date collected|Month|The date when the Record was collected, written as Month, Day, Year or MM/DD/YYYY. (Month must be written first)||
|date collected|Day|The date when the Record was collected, written as Month, Day, Year or MM/DD/YYYY. (Month must be written first)||
|date collected|verbatimEventDate|The date when the Record was collected, written as Month, Day, Year or MM/DD/YYYY. (Month must be written first)||
|field notes|fieldNotes|One of a) an indicator of the existence of, b) a reference to (publication, URI), or c) the text of notes taken in the field about the Event||
|event notes|eventRemarks|Comments or notes about the Event, related to the collection process or some other event in time||



|element|identificationRemarks|The combination of all morphological terms for the Record||
|type status|typeStatus|Nomenclatural types (type status, typified scientific name, publication) applied to the Record||
|higher taxa|higherClassification|A list of taxa/clade ranks superior to order. Do not use punctuation to separate terms. If the identification is uncertain, use term "cf." to describe a similar Taxon. Write 'Indet.' if the Taxon is indeterminable||
|order (suborder)|order|The full scientific name of the order in which the Taxon is classified. Suborder can be listed in paranthesis () if known. If the identification is uncertain, use term "cf." to describe a similar Taxon. Write 'Indet.' if the Taxon is indeterminable||
|family (subfamily)|family|The full scientific name of the family in which the Taxon is classified. Subfamily can be listed in paranthesis () if known. If the identification is uncertain, use term "cf." to describe a similar Taxon. Write 'Indet.' if the Taxon is indeterminable ||
|genus (subgenus) species|genus|The full scientific name of the genus, (subgenus) and species in which the Taxon is classified. If the identification is uncertain, use term "cf." to describe a similar Taxon. Write 'Indet.' if the Taxon is indeterminable||
|genus (subgenus) species|specificEpithet|The full scientific name of the genus, (subgenus) and species in which the Taxon is classified. If the identification is uncertain, use term "cf." to describe a similar Taxon. Write 'Indet.' if the Taxon is indeterminable||
|NULL|scientificName|The full scientific name of the Taxon||
|NULL|identificationQualifier|A brief phrase ("cf.") to express the determiner's doubts about the identification||
|taxon notes|taxonRemarks|Comments or notes about the taxon or name||
|identification by|identifiedBy|A list of names of people or groups who assigned the Taxon to the Record. This is followed by the year (if known) in parantheses on which the Record was identified as representing the Taxon||
|identification by|dateIdentified|A list of names of people or groups who assigned the Taxon to the Record. This is followed by the year (if known) in parantheses on which the Record was identified as representing the Taxon||
|identification notes|identificationRemarks|Comments or notes about the Identification||
|coordinates|verbatimCoordinates|The spatial coordinates of the Location in degrees, minutes, seconds. Written as DD°MM'SS" N, DD°MM'SS" E OR DD°MM.MM' N, DD°MM.MM' E||
|decimmal latitude|decimalLatitude|The geographic latitude (in decimal degrees, using the spatial reference system given in datum field) of the geographic center of a Location. Legal values lie between -90 and 90, inclusive||
|decimal longitude|decimalLongitude|The geographic longitude (in decimal degrees, using the spatial reference system given in datum field) of the geographic center of a Location. Legal values lie between -180 and 180, inclusive||
|datum|geodeticDatum|The ellipsoid, geodetic datum, or spatial reference system (SRS) upon which the geographic coordinates are based||
|georeferenced by|georeferencedBy|A list of names of people or groups who determined the georeference (longitude and latitude) for the Record. This is followed by the year (if known) in parantheses on which the Record was georeferenced||
|georeferenced by|georeferencesDate|A list of names of people or groups who determined the georeference (longitude and latitude) for the Record. This is followed by the year (if known) in parantheses on which the Record was georeferenced||
|georeference notes|georeferenceRemarks|Notes or comments about the spatial description determination||


|NULL|continent|The name of the continent in which the Location occurs||
|country|country|The name of the country or major unit in which the Location occurs||
|state|stateProvince|The name of the state or province unit in which the Location occurs||
|county|county|The name of the county or parish unit in which the Location occurs||
|locality name|verbatimLocality|The specific description of the Location||
|location notes|locationRemarks|Comments or notes about the Location, related to a specific region||
|geologic age|earliestAgeOrLowestAge|The full name of the geochronologic age or chronostratigraphic stage attributable to the stratigraphic horizon from which the cataloged item was collected||
|lithologic notes|lithostratigraphicTerms|The combination of all litho-stratigraphic names for the rock from which the cataloged item was collected||


