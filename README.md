# Developing an African Hub and Search Portal for Scholarly Publishing
- Owned by the African Science community
- Distributed hosting on African territory
- Open source
- Open access
- Free for individual users
- Paid services for institutional users

## Vision and Approach
African research output should be owned and hosted on African territory. We therefore propose an African smart platform and portal for the aggregation of African research output including: 
- African scholarly books 
- Journal articles, preprints, datasets by African scholars and on topics related to Africa
- List of digital African scholarly journals 

The portal will be hosted centrally with an African research-related institution with miorror backups in each of the 5 regions on the continent. To achieve this we will build a decentralized infrastructure with the following features:
- Core distributed data engine with intelligent aggregation and search models
- The data platfrom components are hosted by institutions in African regions (EastA, WestA, NorthA, CentralA)
- A master data intance can be replicated to a cloud service as a matter of backup.
- Number of distributed instances can be increased seamlesly to any country/region in Africa ensuring African ownership
- Utlizing open source distrubted data technologies, big data platforms and AI driven models


## End User Requirements: 
- search content published online with drop down selection (preselections) and/or free choice of content by keywords
- specific to scholarly content by both African scholars and on topics related to the continent and its people
- lowest possible bandwith requirements, quick page load
- eye appealing frontend with African color scheme
- accessibility from every country on the continent (incl. sanctioned nations) to allow for academic freedom
- …


Preprint Repository | Hub and Search Portal 
--- | --- 
[AfricArxiv/preprint-repository](https://github.com/AfricArxiv/preprint-repository) | *as described here*
upload of preprint manuscripts, student reports, research proposals, registered reports/preregistrations, short communications, etc. | aggregating scholarly output from and about Africa via one interface incl preprints form other platforms, scholarly books, datasets for streamlined discoverability | Integrates via API of partner platforms but applying different search scheme atop of their functions
DOI and CC-BY 4.0 attribution | Uses crawling and feature extraction for more accurate semantic context search
integration with Crossref, ORCID, … | Enbales much more search options relevant to content published in relation to Africa as per the sources section below


## Sources of Published Content

### Directories

Scraping content per the term 'Africa' and all by official 54 countries and authors'Ä affiliations at Africna institutions.
Connect to Authors' ORCID and identify African authors and their output 

- contnent from all (currently 6) AfricArXiv partner platforms (OSF, Qeios, ScienceOpen, Figshare, Zenodo, PubPub)

- content from other preprint repositories, 

- [DOAJ](https://doaj.org/search/journals?source=%7B%22query%22%3A%7B%22query_string%22%3A%7B%22query%22%3A%22africa%22%2C%22default_operator%22%3A%22AND%22%2C%22default_field%22%3A%22bibjson.keywords%22%7D%7D%2C%22size%22%3A50%2C%22sort%22%3A%5B%7B%22created_date%22%3A%7B%22order%22%3A%22desc%22%7D%7D%5D%7D)

- [BASEsearch](https://www.base-search.net/Search/Results?lookfor=africa*&name=&oaboost=1&newsearch=1&refid=dcbasen)

- Wikidata / Scholia - https://tools.wmflabs.org/scholia/faq

- [Open Knowledge Maps (uses BASE and/or PubMed)](https://openknowledgemaps.org/map/57bafb92fc16fbcae701e7ef81c77b0a) / possible to integrate the map?

- PubMed / https://www.ncbi.nlm.nih.gov/pubmed/?term=Africa*

paywalled content - if possible with integrations like Knowledge Unlatched and Unpaywall
- https://www.scopus.com/home.uri
- https://clarivate.com/webofsciencegroup/solutions/web-of-science/

#### Repositories
- https://www.connecting-africa.net/index.htm 
- https://info.africarxiv.org/african-digital-research-repositories/

    
### By Type Filtering
- Search by region = Africa* or By other smart features

1) Repositories
- https://v2.sherpa.ac.uk/view/repository_by_country/002.html // API requirements https://v2.sherpa.ac.uk/opendoar/api.html

2) Scholarly Books
- http://www.africanminds.co.za/
- http://www.oapen.org/search?keyword=africa*

3) Journals
- AJOL / https://www.ajol.info/


#### Identify by Author / Article / Publisher / Journal
In the advanced smart search based , crawling and extrating key features related to Africa from sources enables semantic context search with more accurat results. This should take place in follwoing main categories of search criteria or combination of them:

1) Content by African authors / co-authors who are based out in Africa // via [ORCID](https://orcid.org/)

2) Content by African authors / co-authors who are based outside Africa

3) Content by non-African authors / co-authors related to Africa

4) Content authored / co-authored by /for African Institutions

5) Content authored / co-authored by / for one or more African region, city or country

6) Other non-location specific: date, time, topic, publisher, sponsers...etc.


## Languages
- Languages commonly spoken on the continet 
- Machine translations with options/overlay interface to manually improve the text online (see www.GTranslate.io) // GoogleTranspate API
- Language switch // editable by the users and admin


## Technical Specifications
The system consists of three main tiers: The Core Smart Data Platform, Source Data Crowling and Ingestion, Search Intergation and Portal Applications

### The Core Smart Data Platform
- The main engine to mainly store features of content by source publisher incluing the content uploaded directly to the platfrom
- Contains interuim data structires needed for the storing the semnatic features including local ID and source ID to link to the orginal source content when retreving results.
- Stores addtional metadata about the source content to optimize the search process while syncornize online with changes on the source system.
- Pre-cacluates and mainatians updated search metrics triggred by the crolwing and data ingestion process as well as caches the prevouise seaerch results for repeated searches. 

### Source Data Crowling and Ingestion
- Responsible for connecting, parsining and restriving content feastures from external sources by applying the above search idintifers.
- Updates the core data platform continously with new contetn and changes on the exiting content on pre-confirgured time intervales.
- Conduct needed trnafomrations and canconclization on the exterated features and trigger updating interuim search data strtcures and metrics calculations.
- Run a librairy of APIs and Consumers for different appacroches of connectivty to external sources.

### Search Intergation and Portal Applications
- Enbales the end users who would like to use the services to search, retrive, display and anlayze the results by providing search keywords and options.
- Connect and run the semantic context search module on the core data platfrom to retrevie most relvant content and get a list of source idintifiers
- reach out to the source systems to ensure the conent is still intact and recent then restive the content title and abstact as well as other metadata.
- Display the retrived content in different layouts and arrnagments based on customer selection including saving the search and search results for later use.
- Administeration backoffice application for AfricArxiv to be bale to mointor, configure, secure and operate the whole solution.


## Infrastructure Requirements
- The solution should be devloped in incremental appraoch and capatize on contriantization technologies of rease of vertical and horniztal sclability.
- For the first development increment (Proof of Value phase), 5 servers - one at each location - is needed with the following specifictions profile:
   - Operating System: Ubuntu Linux
   - CPU: Intel Xeon 8 Cores x64 3.x GHz
   - Memory: 64 GB
   - Disk: 2 TB SSD or All Flash
   - Networking: Static IP / 10 Gb NIC and Server-grad Internt Connection for external access
   - All other Data Center services
- We might adapt to lower specifictions for first phase if the above are not avilable.
- Identify at least one host institution in each African region that can host the AfricArXiv hub preferably with a data center that is decently opertionalized and uses virtulaization or private cloud.
- Capciaty project for coming 5 years should be provided down the road after completing the first phase so that sounding extimates can be made.
- The design and technical archicture will be made available open source for potential scaling to other African hosting facilities with no need to rebuild or change the solution.


### Using Public Cloud
We can use public cloud hosted and running within Africa for the above main nodes and at the same time we can use a Public Cloud hosted anywhere on the world as a master copy backup for high accessibility. Potential services:
- Microsoft Azure’s services // already in SA
- Amazon Web Services (AWS) // announced to open servers in Africa
- Google Cloud // announced to open servers in Africa


---

Contact us at info@africarxiv.org
