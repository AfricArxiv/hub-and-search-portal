# Developing an African hub and search portal for scholarly communication
- owned by the African Science community
- hosted on African territory
- open source
- open access
- free for users

## Vision
African research output should be owned and hosted on African territory. We therefore propose here an African repository for preprint uploads as well as the aggregation of African research output including: 
- scholarly books 
- journal articles 
- List of digital African scholarly journals 
- …

The portal will be hosted by African research institutions in each of the 5 regions on the continent. To achieve this we will build a decentralized infrastructure with the following features:
- Core database hosted on a server at an African institution
- Mirror backup of the database to servers in all African regions (EastA, WestA, NorthA, CentralA) and a Cloud 
- Ensuring African ownership of African research output
- possibly incl. blockchain components (?)
- …


preprint repository | hub and search portal 
--- | --- 
[AfricArxiv/preprint-repository](https://github.com/AfricArxiv/preprint-repository) | *as described here*
upload of preprint manuscripts, student reports, research proposals, registered reports/preregistrations, short communications, etc. | aggregating scholarly output from and about Africa via one interface inlc preprints form toher platforms, scholarly books, datasets for streamlined discoverability
based on PKP OPS (?) | via API of partner platforms
DOI and CC-BY 4.0 attribution | …
integration with Crossref, ORCID, … | …



## Technical requirements
- ensuring maximum discoverability and interoperability

We are looking at crawling content from three (3) groups:

1) African researchers based on the continent, affiliated to an African research institution 
- seaerch & trivel // crawling approach: 


2) African researchers, not based in Africa, affiliated to a non-African research institution
3) Non-African researchers, who wortk on Africa topics
- search & trivel // crawling approach: 
    
crawling 


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
- provided by/via Ubuntu Net Alliance? / LIBSENSE? / other regional or pan-African entity?



## Languages
- languages commonly spoken on the continet 
- machine translations with options/overlay interface to manually improve the text online (see www.GTranslate.io) // GoogleTranspate API
- Language switch // editable by the users and admin


## Server space
Identify at least one (1) host institutions in each African region that can host the AfricArXiv database.
What capacity is needed in the beginning and projected over the next 3-5 years?


## Connect via cloud services (?)
Make sure that the provider has a server based in Africa. Database must be easy to migrate if needed.
Current cloud options:
- Microsoft Azure’s services // already in SA
- Amazon Web Services (AWS) // announced to open servers in Africa
- Google Cloud // announced to open servers in Africa


---

Contact us at info@africarxiv.org
