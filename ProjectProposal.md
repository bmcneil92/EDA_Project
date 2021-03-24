Brandon McNeil - MTA Project Proposal
Question/need:

My project is intended to gather data for a nonprofit looking to take on the MTA by advocating against fair hikes. This Nonprofit is looking to get some broad insight into current subway users, and see which stations are having relatively high usage. What is the neighborhood make-up of those stations? Can we make any broad assumptions about the users that could help the advocacy group focus on in their attempt to take on the nefarious MTA.

Data Description:

The datasets I will be using to get this information is 12 weeks of MTA Turnstile data from March 2021 to Jan 2021 (http://web.mta.info/developers/turnstile.html).  In addition to this dataset, I aim to tie in Census Data (https://www1.nyc.gov/site/planning/data-maps/open-data/dwn-acs-nta.page) that has been geospatially merged to MTA’s Subway stations. https://data.cityofnewyork.us/Transportation/Subway-Stations/arq3-7z49. From there we can merge this with the MTA Turnstile data to get some information on the neighborhood. 
For the MTA Turnstile data, I will need to aggregate the cumulative value of column header {SCP}, {UNIT}, & {STATION} by {DATE} & {TIME}.
 
Tools:

For Tools used, I will be using SQLite, Python and ArcGIS. ArcGIS will be used to geospatially merge the Census Data and MTA Subway datasets together. No additional geospatial analysis will be needed.

MVP Goal:

The MVP goal for this is to get at least 1 or 2 informative graphs about which subway stations are experiencing relatively high foot traffic, and what neighborhoods / areas of New York City those subway stations are located.
