# DINI AG KIM Working Group Holding Metadata

This repository contains documents of the [DINI AG KIM](https://wiki.dnb.de/display/DINIAGKIM) Working group on **library holding metadata**.

The group was active 2013-2017 and is going to restart in 2023.

## Resources

- Group page (German): https://wiki.dnb.de/x/johZB (with link to mailing list)

- Han at al (2015). *[Exposing library holdings metadata in RDF using schema.org semantics](https://dcpapers.dublincore.org/pubs/article/view/3772)*. Proceedings of DC 2015 conference.

- Scott, D. (2014). *RDFa with schema.org codelab: Library holdings.*
  http://stuff.coffeecode.net/2014/lld_preconference/rdfa_exercises/2_holdings

- BibExtend Community Group. (2014). https://www.w3.org/community/schemabibex/wiki/Holdings and https://www.w3.org/community/schemabibex/wiki/Holdings_via_Offer

- Carsten Klee (2014): *Offene Bestandsdaten und Linked Library Data*
  Talk and slides at https://www.ibi.hu-berlin.de/de/von-uns/bbk/abstracts/ss14/klee
  Includes more references and an analysis of existing standards (Google Sheets somewhere?)
  
   - ISO 20775 - Schema for holdings information
   - ISO 18626 - Interlibrary Loan Transactions
   - Holdings Statements for Bibliographic Items Z39.71-2006
   - MARC21 Holdings
   - ZETA

Holding Ontology Draft (2015):

- https://github.com/dini-ag-kim/holding-ontology
- https://github.com/dini-ag-kim/holding-record
- https://github.com/dini-ag-kim/holding-ontology-examples

- Google Search Recommendations for Book data provided by Libraries:
  https://developers.google.com/search/docs/appearance/structured-data/book#library-systems-and-library-members

[IFLA Library Reference Model (LRM)](https://www.iflastandards.info/lrm)
- "is reproduction item of"/"has reproduction item" and "exemplifies"/"is exemplified by" (Item - Manifestation)
- "is owned by"/"owns" and "was modified by"/"modified" (Item - Agent)
- "has use rights", "has location" (Item - ...)

## Current practice

How does current RDF data provided by library institutions model and expose holding data? (review needed)

### Libraries

- **K10plus**: RDF dump (https://wiki.k10plus.de/display/K10PLUS/Open+Data) does not include holding information. LOD interface uses different URIs and some holding information (e.g. http://uri.gbv.de/document/opac-de-627:ppn:024248908) based in non-standard DAIA Ontology and FRBR. Current work to update the model and data at https://github.com/gbv/k10plus-items

- **DNB**: provides bibliographic data in RDF but no holding information.

- **SLUB Dresden** uses Schema.org (offers/offeredBy), see `curl -s "https://data.slub-dresden.de/resources/1322972605" | jq '.[].offers'` for example.

- **University of Washington Libraries**: see MARC21-to-RDA/LRM/RDF Mapping Project

- ...

### GLAM

Museums and archives have more unique physical objects. This may be somehow related to holdings or it may not

- https://linked.art/ uses CIDOC-CRM

- ...

  

