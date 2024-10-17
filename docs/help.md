# Frequently Asked Questions (FAQ)

## General Questions

### What is Dateno?

Dateno is a dataset search engine designed to help researchers, analysts, developers, journalists, and anyone else find relevant data quickly and efficiently.

### How big is the Dateno index?

As of March 2024, the Dateno index contains 10 million records from 4.9k data catalogs.

### What makes Dateno different from other search engines?

Dateno focuses on speed, advanced filtering options, API access (coming soon), a large index size, and data archiving capabilities.

## Features

### How fast is Dateno?

We've optimized our search functionality using Meilisearch to deliver results as quickly as possible.

### What kind of filters does Dateno offer?

Dateno provides a wide range of filters, including:

- Country
- Subregion
- Macroregion
- Catalog owner
- Catalog owner type
- Catalog type
- Software
- Spoken language
- And more

### Is there an API available?

An API is currently in alpha testing and will be available soon. Please contact us at <dateno@dateno.io> to be notified when beta testing begins.

### Does Dateno archive data?

Yes, we keep all metadata and archive datasets that are at risk of disappearing. This is especially important for open data portals that may be affected by political changes.

## Technical Details

### How does Dateno work?

Dateno is based on the Common Data Index registry of data catalogs. We crawl various data sources using common APIs and export formats, then enrich the data and convert it to a unified structure similar to DCAT.

### What types of data catalogs does Dateno index?

We index a wide range of data sources, including:

- Open data portals
- Geoservers/geoportals
- Scientific data repositories
- Microdata catalogs
- Databases of indicators

### Which software platforms are supported?

Dateno currently supports the following software:

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
- Any software that exports DCAT version 3 standard

## Getting Involved

### My data catalog is not indexed. How can I add it?

If your catalog is not indexed, it may be because:

- It's not in the Common Data Index registry
- It doesn't have any supported API or export format
- There's a connectivity issue (e.g., US IP addresses blocked)

Please contact us at <dateno@dateno.io> if you'd like to see your catalog indexed.

### I want to create a new data catalog that will be indexed by Dateno. Which software should I choose?

Any of the supported software platforms listed above would be suitable. Alternatively, ensure your chosen software exports DCAT version 3 standard.

### How can I report an error or suggest an idea?

Please share your feedback with us at <dateno@dateno.io> or join our Discord community at <https://discord.gg/X4f238ge>.

### Who is behind Dateno?

Dateno is developed by APICrafter Development Ltd., based in Yerevan, Armenia, in collaboration with Open Data Armenia. Our team has been dedicated to open data for over a decade.

## Additional Resources

- [Dateno Blog on Medium](https://medium.com/dateno)
- [Dateno Presentation](https://www.beautiful.ai/player/-Nrp1JiiypOe1exM-Prl/Dateno-2024-03-Public)
- [Reddit post in r/datasets](https://www.reddit.com/r/datasets/comments/1bdn4om/dateno_a_new_dataset_search_engine)

If you have any other questions not covered here, please don't hesitate to contact us at <dateno@dateno.io>.
