This README.txt file was generated on 2024-08-15 by Jessica Guezen 

--------------------
GENERAL INFORMATION
--------------------

1. Title of Dataset: Data from: Interactive effects of climate and land-use gradients on the abundance of arthropod functional groups and trait syndromes in agroecosystems

2. Author Information
	A.	Name: Jessica M. Guezen	
		Institution: University of Guelph
		Email: jessicaguezen@gmail.com

	B.	Name: Madhur Anand
		Institution: University of Guelph
		Email: manand@uoguelph.ca

3. Date of data collection: 2001-2014

4. Geographic location of data collection: Europe

---------------------------
ACCESS INFORMATION
---------------------------

Cited data sets and software used: 

Martin, Emily A. et al. (2019). Data from: The interplay of landscape composition and configuration: new pathways to manage functional biodiversity and agro-ecosystem services across Europe [Dataset]. Dryad. https://doi.org/10.5061/dryad.6tj407n.

Matsuura, K. & Willmott, C.J. (2015a). Terrestrial Air Temperature: 1900-2014 Gridded Monthly Time Series (Version 4.01). Global Air Temperature Archive. Available at: https://climate.geog.udel.edu/. Last accessed 13 August 2024.

Matsuura, K. & Willmott, C.J. (2015b). Terrestrial Precipitation: 1900-2014 Gridded Monthly Time Series (Version 4.01). Global Precipitation Archive. Available at: https://climate.geog.udel.edu/. Last accessed 13 August 2024.

R Core Team. (2024). R: A language and environment for statistical computing.

---------------------
DATA & FILE OVERVIEW
---------------------

1. Code files:

***All R markdown files should be run in order of prefixes***

01_data_access.Rmd: R markdown file with code for downloading climate data and description of download process for land-use and arthropod abundance data (Landscape_Data.csv, Site_Data.csv, Species_Data.csv, Study_Metadata.csv, Trait_Data.csv)

02_spatial.Rmd: R markdown file with code for running spatial analysis. Requires previous run of “01_data_access.Rmd” and the file “Site_Data.csv”

03_data_cleaning.Rmd: R markdown file with code for running data cleaning. Requires previous run of “01_data_access.Rmd” and “02_spatial.Rmd” and the following files: Landscape_Data.csv, Site_Data.csv, Species_Data.csv, Study_Metadata.csv, Trait_Data.csv

04_trait_syndromes.Rmd: R markdown file with code for calculating the percentage of a given trait syndrome across sampling locations. Requires previous run of “01_data_access.Rmd”, “02_spatial.Rmd”, and “03_data_cleaning.Rmd”

04_analysis_poll.Rmd: R markdown file with code for running analysis on pollinator abundance. Requires previous run of “01_data_access.Rmd”, “02_spatial.Rmd”, and “03_data_cleaning.Rmd”

04_analysis_pest.Rmd: R markdown file with code for running analysis on pest abundance. Requires previous run of Requires previous run of “01_data_access.Rmd”, “02_spatial.Rmd”, and “03_data_cleaning.Rmd”

04_analysis_nat.Rmd: R markdown file with code for running analysis on natural enemy abundance. Requires previous run of “01_data_access.Rmd”, “02_spatial.Rmd”, and “03_data_cleaning.Rmd”

04_analysis_poll_ts1.Rmd: R markdown file with code for running analysis on diet generalist pollinator abundance. Requires previous run of “01_data_access.Rmd”, “02_spatial.Rmd”, and 
“03_data_cleaning.Rmd”

04_analysis_poll_ts2.Rmd: R markdown file with code for running analysis on diet specialist pollinator abundance. Requires previous run of “01_data_access.Rmd”, “02_spatial.Rmd”, and “03_data_cleaning.Rmd”

04_analysis_pest_ts1.Rmd: R markdown file with code for running analysis on habitat generalist pest abundance. Requires previous run of “01_data_access.Rmd”, “02_spatial.Rmd”, and “03_data_cleaning.Rmd”

04_analysis_pest_ts2.Rmd: R markdown file with code for running analysis on habitat specialist pest abundance. Requires previous run of “01_data_access.Rmd”, “02_spatial.Rmd”, and “03_data_cleaning.Rmd”

04_analysis_nat_ts1.Rmd: R markdown file with code for running analysis on habitat generalist, flight dispersal natural enemy abundance. Requires previous run of “01_data_access.Rmd”, “02_spatial.Rmd”, and “03_data_cleaning.Rmd”

04_analysis_nat_ts2.Rmd: R markdown file with code for running analysis on habitat generalist, ground dispersal natural enemy abundance. Requires previous run of “01_data_access.Rmd”, “02_spatial.Rmd”, and “03_data_cleaning.Rmd”

04_analysis_nat_ts3.Rmd: R markdown file with code for running analysis on habitat specialist, ground dispersal natural enemy abundance. Requires previous run of “01_data_access.Rmd”, “02_spatial.Rmd”, and “03_data_cleaning.Rmd”

05_figures: R markdown file with code for all figures in manuscript. Requires previous run of all other R markdown files


---------------------------
METHODOLOGICAL INFORMATION
---------------------------

1. Description of methods used for collection of data: See Martin et al. (2019), Matsuura, K. & Willmott, C.J. (2015 a & b) for descriptions of data collection.


2. Methods for processing the data: See R Markdown files for data processing descriptions


3. Software needed to interpret the data: All analyses were run in R version 4.4.0 (R Core Team 2024)

