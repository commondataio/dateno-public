# FAQ

## What is Dateno?

Dateno is a dataset search engine. It's intended to help researchers, analysts, developers, journalists and everyone else to find relevant data.

Dateno is ready for your everyday data search.

## How big is Dateno index?

Dateno index has 6.9 millions records from 2.5k data catalogs in the end of 2023. 


## What makes Dateno different?

In short our focus is speed, filters, API, index size and data archive. 

### Speed
We focused on a lot to provide search so fast as possible. We use Meilisearch as search engine and use it to deliver search results ASAP. 

### Filters
Dateno has a huge number of filters: by country, subregion, macroregion, catalog owner, catalog owner type, catalog type,software, spoken language and etc. 

### API

Dateno index is open to use as API. Right now it's alpha testing and will be available soon. Please write us at dateno@dateno.io and we will provide access when beta testing will start.

### Index size

Our index is growing fast and It will grow significantly when we will index major online data portals, huge scientific research repositories with custom APIs and major public indicators databases. 

### Data archive

Data portals disappear, data disappear and too often it's not saved anywhere since data files are big or not indexable by Google, Internet Archive, Bing, Common Crawl and other search engines. We keep all metadata and we will archive datasets under risk. It's especially important for open data portals that disappear on political changes in certain countries.

## How Dateno works ?

Dateno based on Common Data Index registry of the data catalogs. It's about 9900+ data catalogs with lot's of metadata about each catalog. 

Dateno crawls open data portals, geoservers/geoportals, scientific data repositories, microdata catalogs, databases of indicators and other data catalogs. So we have datasets, map layers and indicators and all of them considered as datasets.

Websites crawled using common API and export formats like DCAT, CKAN API, CSW, WFS, WMS, ArcGIS Rest API and many others. 

After crawl we enrich data and convert it to the unified structure similar to DCAT as single search index. 

Search index is available as Meilisearch search index and internal  NoSQL database. 

## My data catalog not indexed. How to add it ?

If catalog is not indexed it means that:
- it's not in the Common Data Index registry
- or it haven't any supported API or export format to index it
- or there is some connectivity issue. For example US IP addresses blocked

Please contact us dateno@dateno.io if you would like to see your catalog indexed too.

## I want to create a new data catalog that will be indexed by Dateno. Which software I should choose ?

Currently Dateno supports following software:
- CKAN
- DKAN
- Socrata
- OpenDataSoft
- uData
- Geonetwork
- Geonode
- Dataverse
- InvenioRDM
- NADA
- ArcGIS Hub
- ArcGIS Server

And any software that exports [DCAT version 3](https://www.w3.org/TR/vocab-dcat-3/) standard.


# I've got an error or idea, how to contact you ?

Please share it with as at dateno@dateno.io or using Discord https://discord.gg/X4f238ge

# Who is behind Dateno ?

We are APICrafter Development Ltd., Armenia, Yerevan and Open Data Armenia. Our team dedicated to open data more than 10 years and we would like to create a project that will help everyone who is searching for open data around the world.

