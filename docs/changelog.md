# Changelog

Dateno project and subprojects unified changelog.

## 0.0.2 - 2024-03-14

### New datasets

* Added World Bank data.worldbank.org indicators, about 4.8M
* Added indicators from all known instantances of PxWeb statistics software
* Added datasets from Aleph (OCCRP and etc) data catalogs

### UI

* Added social sharing buttons
* Added ProductHunt badge
* Integrated Common Data Index registry as Dateno Registry at dateno.io/registry
* Updated Dateno Registry styles

## API and backend 

* Added new filter "Data type" with *dataset.datatype* field
* Replaced *dataset.formats* with autodetected values starting with dot
* Added autodetected mime and extensions to *resources* as "*d_mime*" and "*d_ext*"
* Updated Meilisearch up to 1.7.1 version (faster indexing, less space used) 
* Rebuilded search index,

### Data catalogs registry

* Renamed Common Data Index registry to Dateno Registry
* Updated metadata of the almost PxWeb installations 
* Added multiple Hyrax and Esploro based data catalogs
* Added many new scientific data catalogs in China 
* Fixed many typos using builder "validate" command

## 0.0.1 - 2024-03-13

### Added

* First version released
* Added search index with basic 
