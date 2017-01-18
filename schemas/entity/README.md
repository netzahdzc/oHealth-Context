# Health issues tracking data models

These data models allow to perform civic issue tracking. They have been designed with a view to enabling trivial interoperability between FIWARE NGSI version 2 and Open311. As a result, property names have not been normalized to the camelCasesyntax, they remain as currently specified by Open311. That is the rationale behind naming entity types with Open311 as prefix. However, a few properties are added, so that FIWARE NGSI version 2 implementations can properly store and serve Open 311 data.

FIWARE and OASC, in the medium term, might propose to the Open311 Community a harmonized data model aligned with the rest of FIWARE data models and schema.org. In fact, using these data models and a FIWARE NGSI version 2 implementation it is trivial to implement the APIs proposed by Open311. Another option would be the use of JSON-LD to define equivalencies and mappings between a FIWARE / Schema.org data model and Open 311.



