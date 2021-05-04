<a href="https://covid19dataproject.org/">
    <img src="https://covid19dataproject.org/wp-content/uploads/2020/04/LOGO-Broadstreet-covid19.svg" alt="Broadstreet logo" title="BroadStreet" align="right" height="80" />
</a>

Broadstreet COVID-19 Data Project
=================================

## Vaccine Data Tracking

The COVID-19 Data Project was created in March 2020 to satisfy the driving need for accessible data tracking of the spread of the coronavirus across the United States. Initially starting with the collection of cumulative case counts of COVID-19 and mortalities in the United States and its territories, at the county-level, the COVID-19 Data Project has since expanded to include analysis of policies relating to COVID-19, collection of cumulative case counts by race and ethnicity, and various intern-led research projects relating to the COVID-19 pandemic. That information can be found here: 
* [COVID-19 Data Project Home] (https://covid19dataproject.org/)
* [Daily Numbers] GitHub (https://github.com/BroadStreet-Health/daily-numbers)
* [Policy] GitHub (https://github.com/BroadStreet-Health/policy)
* [Special Interest Projects Gallery] (https://covid19dataproject.org/special-interest-projects/)

The newest expansion of the COVID-19 Data Project is focused on vaccine administration at the state- and county-level across the United States, hereon referred to as Vaccine Data Tracking. 

The [United States Food and Drug Administration authorized public use of the first COVID-19 vaccine] (https://www.fda.gov/news-events/press-announcements/fda-takes-key-action-fight-against-covid-19-issuing-emergency-use-authorization-first-covid-19) in December of 2020. The Pfizer vaccine was the first approved, and clinical trials found it to be 95% effective in prevention. The approval of the Pfizer vaccine was followed by an emergency authorization of the [Moderna COVID-19 vaccine on December 18th, 2020] (https://www.fda.gov/emergency-preparedness-and-response/coronavirus-disease-2019-covid-19/moderna-covid-19-vaccine#:~:text=On%20December%2018%2C%202020%2C%20the,SARS%2DCoV%2D2). The Moderna vaccine was found to be 94.1% effective in preventing infection via clinical trials. The third vaccine approved for emergency use in the United States was [Johnson & Johnson’s single-shot coronavirus vaccine] (https://www.washingtonpost.com/health/2021/02/26/johnson-and-johnson-vaccine-fda/), which was approved in February. The [Johnson & Johnson vaccine was found to be 66.3% effective in prevention via clinical trials] (https://www.cdc.gov/coronavirus/2019-ncov/vaccines/different-vaccines/janssen.html).   

As vaccines began to be approved for use, health departments were advised in a [12/22/20 interim recommendation by the Advisory Committee on Immunization Practices and the Centers for Disease Control] (https://www.cdc.gov/mmwr/volumes/69/wr/mm695152e2.htm) to roll-out vaccine administration in phases, prioritizing front-line health workers and those in long-term care facilities. The phased approach was introduced due to the limited quantity of doses available. As vaccine administration continued to roll-out, the need for aggregate collection of vaccine administration at the county-level was needed, and the Vaccine Data Tracking team for the COVID-19 Data Project was created mid-March.    

The Vaccine Data Tracking Project is unique in that it is one of the only datasets collecting vaccine administration data at the county-level across the United States. This team was created in March of 2021 as states and health departments began administering vaccines and reporting information regarding administration. State dashboards were assessed to determine if information regarding vaccine administration was being reported and if county-level information was available. States were then categorized by the rate at which they update their data (i.e. daily, weekly, monthly, presence of historical data), and data collection began on 18 out of the identified 50 states, plus Puerto Rico and DC. This data allows for visualization of how vaccination administration is occurring throughout the United States. This data gives the public knowledge regarding the rate of vaccination across the United States. The data will be updated monthly and is available to be downloaded for further analysis as a .csv or .xlsx file.  


### Structure of the Dataset

The data is structured in wide form. This is how the first dose in the United States would be represented at the county level for April 1, 2021: 05000US06001, Alameda County California, CA, 1, 0, 0, 1. This is how the first dose would be represented at the state level: 04000US06, California(state), CA, 1, 0, 0, 1. Both the county and state data begin with the state/county, followed by the state identification number/county identification number. At both the state and the county level, the data recorded are first doses, followed by the number of second doses, the number of single doses, then the number of total doses. At the top of each state, there is a state totals row and then a row with the state name. The state totals row is taken directly from the state dashboard. The row with the state name is calculated by the sum of the county information for that respective state. 
Variables used in our data include:
* 1st Dose_: one dose of a COVID-19 vaccine received/administered 
* 2nd Dose_: two doses of a two-dose series of COVID-19 vaccine received/administered or fully vaccinated
* Single Dose_: one dose of a single dose COVID-19 vaccine administered
* Total Doses_: total number of doses administered

Each state varies in how they define each variable and how they categorize single-dose vaccines. In order to account for those differences, we went through each dashboard and consolidated their definitions into one spreadsheet and attempted to standardize the definitions as much as possible. Dashboards will be reviewed on a monthly basis to reverify definitions and capture any changes that may not have been apparent when completing data entry.  


Table 1. Variable Definitions by State