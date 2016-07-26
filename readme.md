#Paleontology Database Documentation

Repository for ANSP Vertebrate Paleontology database. Intended for use by lab volunteers and co-op students entering data for Vertebrate Paleontology. 

> This table describes all the fields currently used in the database. It is a reference for entering data correctly and using the correct vocabulary or structure each fields requires. Controlled vocabulary is very important to make sure that records are acurrate and can be used for other programs. 

> The first column 'FileMaker' is the name of the column in FileMaker.

> The second column 'Darwin Core Field' is the name of the matching fields used by the Darwin Core standards (http://rs.tdwg.org/dwc/terms/index.htm). This is important when the data is added to external projects like iDigBio (https://www.idigbio.org/) or larger databases within the Academy.

> The third column 'Definition' describes the use of that column and what data should be entered into the field. This may seem obvious for something like Catalog Number, but can be confusing when trying to differentiate between identification notes and taxon notes. Whenever in doubt about where to add new data, consult the definitions of each field and choose appropriately.

> The fourth and final column 'Example' provides examples of expected data for that field and how it should be written. For fields such as Collector, where the data can invole multiple people and initials, it is very important to follow the rules and enter the data as described here. When this data is exported for other projects it expects the data to be written correctly and can result in errors if it is not. Some fields may ask for the same information twice and it is useful to look at the examples to understand what is needed in each field. For example, Coordinates should contain the Latitude and Longitude written in a specific way, while Latitude and Longitude should only be written as decimal degrees if known.

------

| FileMaker Field | Corresponding Darwin Core Field | Definition | Example |
|---|---|---|---|
| catalog ID ||||
| catalog # ||||
| element ||||
| count ||||
| type status ||||
| higher taxa ||||
| order (suborder) ||||
| family (subfamily) ||||
| genus (subgenus) species ||||
| identification by ||||
| taxon notes ||||
| identification notes ||||
| preparation notes ||||
| collectors ||||
| coordinates ||||
| latitude ||||
| longitude ||||
| datum ||||
| georeferenced by ||||
| georeference notes ||||
| field # ||||
| field notes ||||
| date collected ||||
| country ||||
| locality name ||||
| location notes ||||
| event notes ||||
| occurrence notes ||||
| geologic age ||||
| lithologic notes ||||
| collection ||||
| disposition ||||
| media ||||
| references ||||
| citation ||||
| created ||||
| created by ||||
| modified ||||
| modified by ||||
| other information ||||

This repository was written by Vincent O'Leary as part of my co-op at the Academy of Natural Sciences (ANSP)