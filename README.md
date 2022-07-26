FWS-Endangered-Species-PDA
Python Data Analysis Project on FWS Endangered Species List

Problem Description:
The earth is currently experiencing its 6th mass extinction. During the past five, Ninety-nine percent of all species that have ever lived have gone extinct. Now, the rate of extinction is occurring 1,000 to 10,000 times faster. (Cho)
This crisis, unlike past extinctions can be linked to climate change, land use change, invasive species introduction, pollution, and resource exploitation. To protect the further loss of species, the ESA was passed in 1973 which was meant to help imperiled species recover from the brink of extinction. But the species protections and regulations have been weakened due to industrial and economic pressures. (Bleau)

Although its difficult to accurately put a cost on the loss of species, the global value of ecosystem services was estimated to average $46 trillion per year in 2007 according to Costanza et al. With this estimate, the cost of lost species is likely even higher today. 

Data Science Project Scoping: 
The focus of this project is the Global mass exctinction crisis and species listed under the Endangered Species Act (ESA). I will be using data from the Fish and Wildlife Service (FWS) which will include listed species under the ESA, species of concern, listed species with recovery plans, and the FY 2017 and FY 2018 expenditures. In the future I would like to compare expenditures from additional years to see if there is a trend in the data, but 2018 was the most recent expenditures available on the FWS site.  

FWS Species Data Explorer Metadata -
	Group: The taxonomic Group the species belongs to.
	Status: The specific status of this entity as it relates to its status category and the ESA. https://ecos.fws.gov/ecp0/html/db-status.html
	Scientific Name: The scientific name of the species. If the species is listed under the ESA, the name is displayed as it is shown in the listing document. Each value is hyper-linked to the ECOS species profile report.
	Common Name:  The common name of the species. If the species is listed under the ESA, the name is displayed as it is shown in the listing document.
	Location: An indication of whether the species is Foreign or Domestic or Both.
	Status Category: The general status (i.e. category) of this entity as it relates to the ESA.
		Listed: The species entity is listed under the U.S. Endangered Species Act.
		Candidate for Listing: The species entity is a Candidate for Listing.
		Delisted: The species entity was listed under the ESA, but is now delisted.
		Proposed for Listing: TODO
		Proposed for Status Change or Delisting: TODO
		Petitioned for Listing, Under Review: TODO
	Listing Date:  The effective date of the listing as published in Title 50 of the Code of Federal Regulations (CFR), parts 17.11 and 17.12. This field will be null if the species entity has not been listed.
	Inverted Common Name: The inverted common name of the species. If the species is listed under the ESA, the name is displayed as it is shown in the listing document.
	Area: The description of the distinct population segment. Only non-null if the record's 'Distinct Population Segment?' value is true.

FWS Species Recovery Plan Data Explorer Metadata -
	Group: The taxonomic Group the species belongs to.
	Status: The specific status of this entity as it relates to its status category and the ESA. https://ecos.fws.gov/ecp0/html/db-status.html
	Scientific Name: The scientific name of the species. If the species is listed under the ESA, the name is displayed as it is shown in the listing document. Each value is hyper-linked to the ECOS species profile report.
	Common Name:  The common name of the species. If the species is listed under the ESA, the name is displayed as it is shown in the listing document.
	Recovery Actions: Number of recovery actions associated with species.
        Recovery Document Date: Date in a format used to sort.
	Region: Name of the region the species is in. https://www.fws.gov/about/regions
	Area: The description of the distinct population segment. Only non-null if the record's 'Distinct Population Segment?' value is true.

FWS Federal and State Endangered and Threatened Species Expenditures Metadata-
	Group: The taxonomic Group the species belongs to.
	Status: The specific status of this entity as it relates to its status category and the ESA. https://ecos.fws.gov/ecp0/html/db-status.html
	Scientific Name: The scientific name of the species. If the species is listed under the ESA, the name is displayed as it is shown in the listing document. Each value is hyper-linked to the ECOS species profile report.
	Inverted Common Name: The inverted common name of the species. If the species is listed under the ESA, the name is displayed as it is shown in the listing document.
	FWS 2017: Total FWS 2017 expenditures for the species population.
	Other Fed 2017: Total 2017 expenditures combined from 27 Federal agencies (not including FWS) for the species population.
        States 2017: Total State 2017 expenditures for the species population.
	Total 2017: Total combined 2017 expenditures for the species population.
	Area: The description of the distinct population segment. Only non-null if the record's 'Distinct Population Segment?' value is true.
	FWS 2018: Total FWS 2018 expenditures for the species population.
	Other Fed 2017: Total 2018 expenditures combined from 27 Federal agencies (not including FWS) for the species population.
        States 2018: Total State 2018 expenditures for the species population.
	Total 2018: Total combined 2018 expenditures for the species population.
	
Who or what is affected by this problem?
- Everyone,
- Ecosystems,
- Industries and financial markets

Why is solving this problem a priority?
- Financial cost/value of provided services,
- Protection of ecosystem services,
- Protection from our own extinction
	
What other groups/stakeholders need to be involved in scoping and implementing this project?
- Policy makers,
- Corporations (corporate accountability),
- Consumers

Goals:
- Highlight discrepancies between highly - funded and less-funded/non-funded species (equity),
- Highlight need for ESA funding (effectiveness),
- Highlight the cost of extinction (efficiency)

Data analysis:
- EDA of categorical variables (group, listing status, )
- Look at distributions
- EDA of numerical variables (compare fws / total spending per group, compare  fws / total spending between top funded and least funded. 
- Do the top funded have anything in common?
- Is there a correlation between species budget and recovery plans?
- Correlation between budget and number of recovery actions?

Future ideas: 
- Highlight how many species are petitioned/ how long they have been on waiting list,
- How many years has (subset of species) been listed? (effectiveness of listing/protection) 

Citations:

Bleau, Katie. “Biodiversity on the Brink: The Consequences of a Weakened Endangered Species Act.” Yale Environment Review, 23 Jan. 2020, https://environment-review.yale.edu/biodiversity-brink-consequences-weakened-endangered-species-act. 

Cho, Renee.  “Why Endangered Species Matter.” State of the Planet, 3 Apr. 2019, https://news.climate.columbia.edu/2019/03/26/endangered-species-matter/#:~:text=%E2%80%9CEven%20if%20it's%20not%20a,that%20ecosystem%20to%20stop%20working.%E2%80%9D. 

Costanza, Robert, et al. “Changes in the Global Value of Ecosystem Services.” Global Environmental Change, vol. 26, May 2014, pp. 152–158., https://doi.org/10.1016/j.gloenvcha.2014.04.002. 

Lien, Aaron M., et al. “Opportunities and Barriers for Endangered Species Conservation Using Payments for Ecosystem Services.” Biological Conservation, vol. 232, Apr. 2019, pp. 74–82., https://doi.org/10.1016/j.biocon.2019.01.017. 

“Summary of the Endangered Species Act.” EPA, Environmental Protection Agency, 28 Sept. 2021, https://www.epa.gov/laws-regulations/summary-endangered-species-act. 
