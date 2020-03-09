# Developing an African Hub and Search Portal for Scholarly Publishing
- Owned by the African Science community
- Distrbuted hosting on African territory
- Open source
- Open access
- Free for users

## Vision
African research output should be owned and hosted on African territory. We therefore propose here an African smart platform and portal for preprint uploads as well as the aggregation of African research output including: 
- Scholarly books 
- Journal articles 
- List of digital African scholarly journals 
- …

The portal will be hosted by African research institutions in each of the 5 regions on the continent. To achieve this we will build a decentralized infrastructure with the following features:
- Core distributed data engine with intillegint aggrigation and search models
- The data platfrom components are hosted by intritutaions in African regions (EastA, WestA, NorthA, CentralA)
- A master data intance can be replicated to a cloud service as a matter of backup.
- Number of districbuted instances can be increased seamlesly to any country/region in Africa ensuring African ownership
- Utlizing distrubted data technologies, big data platforms and AI driven models


preprint repository | hub and search portal 
--- | --- 
[AfricArxiv/preprint-repository](https://github.com/AfricArxiv/preprint-repository) | *as described here*
upload of preprint manuscripts, student reports, research proposals, registered reports/preregistrations, short communications, etc. | aggregating scholarly output from and about Africa via one interface inlc preprints form toher platforms, scholarly books, datasets for streamlined discoverability
based on PKP OPS (?) | Integrates via API of partner platforms but applying different search sechme atop of thier functions
DOI and CC-BY 4.0 attribution | Uses crowling and feature extraction for more accurate search results
integration with Crossref, ORCID, … | Enbales much more search oprtions relvent to content pulish in relation to Africa as per the sources section below



## Technical requirements
- ensuring maximum discoverability and interoperability
- …
- …

## Sources

### Directories

- [DOAJ](https://doaj.org/search?ref=homepage-box&source=%7B%22query%22%3A%7B%22query_string%22%3A%7B%22query%22%3A%22africa*%22%2C%22default_operator%22%3A%22AND%22%7D%7D%7D)

- [BASEsearch](https://www.base-search.net/Search/Results?lookfor=africa*&name=&oaboost=1&newsearch=1&refid=dcbasen)

- Wikidata / Scholia - https://tools.wmflabs.org/scholia/faq

- [Open Knowledge Maps (uses BASE or PubMed)](https://openknowledgemaps.org/map/57bafb92fc16fbcae701e7ef81c77b0a) / possible to integrate the map?

- PubMed / https://www.ncbi.nlm.nih.gov/pubmed/?term=Africa*

paywalled // therefore ignore??
- https://www.scopus.com/home.uri
- http://wokinfo.com/

    
### by type
- search by region = Africa*

1) Repositories
- https://v2.sherpa.ac.uk/view/repository_by_country/002.html // API requirements https://v2.sherpa.ac.uk/opendoar/api.html

2) Scholarly Books
- http://www.africanminds.co.za/
- http://www.oapen.org/search?keyword=africa*

3) Journals
- AJOL / https://www.ajol.info/


#### identify by author / article / publisher / journal
We are looking at crawling content from three (3) groups:
1) African researchers based on the continent, affiliated to an African research institution 
- seaerch & trivel // crawling approach: 

2) African researchers, not based in Africa, affiliated to a non-African research institution

3) Non-African researchers, who wortk on Africa topics
- search & trivel // crawling approach: …


# database with the following features / semantic
- local identifier
- ID source of publication // DOI - via crossref or other

- African university / research institute
- language
- (other metadata)


# approach
distributed crawling & passing on a regional basis: 
the automated crawling will be implemented on a regional / national level to be time and cost sensitive/efficient


# end user requirements: 
- be able to search content published online with drop down selection and/or free chouce of keywords
- specific to African scholarly content


# server space requirements
starting at XXX GB
- provided by/via Ubuntu Net Alliance (?) / LIBSENSE (?) / TENET (?) / other regional or pan-African entity?

Identify at least one (1) host institution in each African region that can host the AfricArXiv database.
What capacity is needed in the beginning and projected over the next 3-5 years?


## Connect via cloud services (?)
Make sure that the provider has a server based in Africa. Database must be easy to migrate if needed.
Current cloud options:
- Microsoft Azure’s services // already in SA
- Amazon Web Services (AWS) // announced to open servers in Africa
- Google Cloud // announced to open servers in Africa


# Languages
- languages commonly spoken on the continet 
- machine translations with options/overlay interface to manually improve the text online (see www.GTranslate.io) // GoogleTranspate API
- Language switch // editable by the users and admin




---

Contact us at info@africarxiv.org
