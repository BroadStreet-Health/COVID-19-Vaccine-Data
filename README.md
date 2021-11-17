<a href="https://covid19dataproject.org/">
    <img src="https://covid19dataproject.org/wp-content/uploads/2020/04/LOGO-Broadstreet-covid19.svg" alt="Broadstreet logo" title="BroadStreet" align="right" height="80" />
</a>

Broadstreet COVID-19 Data Project
=================================

## Vaccine Data Tracking
The COVID-19 Data Project was created in March 2020 to satisfy the driving need for accessible data tracking of the spread of the coronavirus across the United States. Initially starting with the collection of cumulative case counts of COVID-19 and mortalities in the United States and its territories, at the county-level, the COVID-19 Data Project has since expanded to include analysis of policies relating to COVID-19, collection of cumulative case counts by race and ethnicity, and various intern-led research projects relating to the COVID-19 pandemic. That information can be found here: 

* [COVID-19 Data Project Home](https://covid19dataproject.org/)
* [Daily Numbers](https://github.com/BroadStreet-Health/daily-numbers) GitHub 
* [Policy](https://github.com/BroadStreet-Health/policy) GitHub 
* [Health Equity](https://github.com/BroadStreet-Health/Race-and-Ethnicity-Data) GitHub
* [Special Interest Projects Gallery](https://covid19dataproject.org/special-interest-projects/)

The newest expansion of the COVID-19 Data Project is focused on vaccine administration at the state-and county-level across the United States, hereon referred to as Vaccine Data Tracking. 

The [United States Food and Drug Administration authorized public use of the first COVID-19 vaccine](https://www.fda.gov/news-events/press-announcements/fda-takes-key-action-fight-against-covid-19-issuing-emergency-use-authorization-first-covid-19) in December of 2020. The Pfizer vaccine was the first approved, and clinical trials found it to be 95% effective in prevention. The approval of the Pfizer vaccine was followed by an emergency authorization of the [Moderna COVID-19 vaccine on December 18th, 2020](https://www.fda.gov/emergency-preparedness-and-response/coronavirus-disease-2019-covid-19/moderna-covid-19-vaccine#:~:text=On%20December%2018%2C%202020%2C%20the,SARS%2DCoV%2D2). The Moderna vaccine was found to be 94.1% effective in preventing infection via clinical trials. The third vaccine approved for emergency use in the United States was [Johnson & Johnson’s single-shot coronavirus vaccine](https://www.washingtonpost.com/health/2021/02/26/johnson-and-johnson-vaccine-fda/), which was approved in February. The [Johnson & Johnson vaccine was found to be 66.3% effective in prevention via clinical trials](https://www.cdc.gov/coronavirus/2019-ncov/vaccines/different-vaccines/janssen.html).   

As vaccines began to be approved for use, health departments were advised in a [12/22/20 interim recommendation by the Advisory Committee on Immunization Practices and the Centers for Disease Control](https://www.cdc.gov/mmwr/volumes/69/wr/mm695152e2.htm) to roll-out vaccine administration in phases, prioritizing front-line health workers and those in long-term care facilities. The phased approach was introduced due to the limited quantity of doses available. As vaccine administration continued to roll-out, the need for aggregate collection of vaccine administration at the county-level was needed, and the Vaccine Data Tracking team for the COVID-19 Data Project was created mid-March.    

[As of 05/12/21, eligibility to receive the COVID-19 vaccine in the United States expanded to everyone 12 and older](https://www.usnews.com/news/best-states/articles/covid-19-vaccine-eligibility-by-state)  starting with the Pfizer vaccine. [As of 10/25/21, 57% of the United States’ population has been fully vaccinated, with 66% having received at least one dose.](https://www.cdc.gov/coronavirus/2019-ncov/vaccines/index.html). Although more than half of U.S. adults are now fully vaccinated against the coronavirus, the speed of the vaccine rollout has slowed.  

Variant strains of COVID-19 have been reported globally with [five variants](https://www.cdc.gov/coronavirus/2019-ncov/variants/variant.html?CDC_AA_refVal=https%3A%2F%2Fwww.cdc.gov%2Fcoronavirus%2F2019-ncov%2Ftransmission%2Fvariant.html) being of concern in the United States: B.1.1.7 (Alpha) first identified in the United Kingdom, B.1.351 (Beta) emerging out of South Africa, P.1 (Gamma) initially detected in Brazil, B.1.427 and B.1.429 (Epsilon) both originating from California, and B.1.617.2 (Delta) initially identified in India; these variants appear to spread more easily and have potential to put increased strain on healthcare systems. As the virus is still developing, plans for a [third booster dose](https://www.fda.gov/news-events/press-announcements/fda-brief-fda-hold-advisory-committee-meeting-discuss-pfizer-biontechs-application-covid-19-booster) for the Pfizer and Moderna vaccines, and a second booster dose for the Johnson & Johnson vaccine, are in play, with plans to roll out booster doses in Fall 2021.

[As of 9/22/2021, the FDA amended the emergency use authorization for the Pfizer COVID-19 Vaccine to allow for use of a single booster dose to be administered at least six months after completion of the primary series.](https://www.fda.gov/news-events/press-announcements/fda-authorizes-booster-dose-pfizer-biontech-covid-19-vaccine-certain-populations) On October 20, 2021 the FDA took action to expand the use of booster dose for COVID-19 vaccines in eligible populations. This amendment allows for the use of a single booster dose as follows: 1) a single booster dose of Moderna COVID-19 vaccine to be administered six months after completion of the primary series; 2) a single booster of the Janssen vaccine to be administered two months after completion of a primary regimen; 3) the use of each available COVID-19 vaccine as a heterologous booster dose.        

The Vaccine Data Tracking Project is unique in that it is one of the only datasets collecting vaccine administration data at the county-level across the United States. This team was created in March of 2021 as states and health departments began administering vaccines and reporting information regarding administration. State dashboards were assessed to determine if information regarding vaccine administration was being reported and if county-level information was available. States were then categorized by the rate at which they update their data (i.e. daily, weekly, monthly, presence of historical data), and data collection began on 18 out of the identified 50 states, plus Puerto Rico and DC. This data allows for visualization of how vaccination administration is occurring throughout the United States. This data gives the public knowledge regarding the rate of vaccination across the United States. The data will be updated monthly and is available to be downloaded for further analysis as a .csv or .xlsx file.  

## Structure of the Dataset
The data is structured in wide format. This is how the first dose in the United States would be represented at the county level for April 1, 2021: 05000US06001, Alameda County California, CA, 1, 0, 0, 1. This is how the first dose would be represented at the state level: 04000US06, California(state), CA, 1, 0, 0, 1. Both the county and state data begin with the state/county, followed by the state identification number/county identification number. At both the state and the county level, the data recorded are first doses, followed by the number of second doses, the number of single doses, then the number of total doses. At the top of each state, there is a state totals row and then a row with the state name. The state totals row is taken directly from the state dashboard. The row with the state name is calculated by the sum of the county information for that respective state. 
Variables used in our data include:
* 1st Dose_: one dose of a COVID-19 vaccine received/administered 
* 2nd Dose_: two doses of a two-dose series of COVID-19 vaccine received/administered or fully vaccinated
* Single Dose_: one dose of a single dose COVID-19 vaccine administered
* Additional Dose_: vaccination doses administered after completion of a primary vaccine series
* Total Doses_: total number of doses administered

Each state varies in how they define each variable and how they categorize single-dose vaccines. In order to account for those differences, we went through each dashboard and consolidated their definitions into one spreadsheet and attempted to standardize the definitions as much as possible. Dashboards will be reviewed on a monthly basis to reverify definitions and capture any changes that may not have been apparent when completing data entry.  

Table 1. Variable Definitions by State
<table>
	<tr>
		<th>State<th>
		<th>First Dose<th>
		<th>Second Dose<th>
		<th>Single Dose<th>
<th>Additional Dose<th>
		<th>Total Doses<th>
	</tr>
	<tr>
		<td>Alabama<td>
		<td>Number of people receiving one or more doses includes those receiving any dose (first or second dose of either Pfizer-BioNTech or Moderna vaccine and those receiving the 1 dose of the single shot of the Johnson & Johnson (J&J) Janssen vaccine).<td>
 		<td>Number of people who have completed vaccine series includes those who received the second dose of either the Pfizer-BioNTech or Moderna vaccine and those who received 1 dose of the single-shot of Johnson & Johnson (J&J) Janssen. This means that doses of J&J will be counted in both categories of number receiving one or more doses and fully vaccinated/completed vaccine series. Anyone looking at these metrics should not add the two together to get the total doses administered. The "fully vaccinated" totals are  subset of the "Number of people receiving one or more doses"<td>
		<td>Total number of Johnson doses administered<td>
<td>N/A<td>
		<td>Doses Administered is the cumulative count of individual COVID-19 vaccine doses, including first and second doses, administered by Alabama providers as reported by the providers in ImmPRINT<td>
	</tr>
	<tr>
		<td>Alaska<td>
		<td>People with at least one dose<td>
 		<td>People fully vaccinated<td>
		<td>N/A<td>
<td>N/A<td>
		<td>Total doses administered<td>
	</tr>
<tr>
		<td>Arizona<td>
		<td>Number of people who have received at least one dose is the number of unique individuals who have received COVID-19 vaccine.<td>
 		<td>Number of people fully vaccinated is the number of people who received a valid, complete vaccine series.<td>
		<td>N/A<td>
<td>N/A<td>
		<td>Total number of COVID-19 vaccine doses administered<td>
	</tr>
	<tr>
		<td>Arkansas<td>
		<td>People with at least one dose<td>
 		<td>People fully vaccinated<td>
		<td>N/A<td>
<td>N/A
		<td>Doses Given <td>
	</tr>
	<tr>
		<td>California<td>
		<td>Cumulative at least one dose. Cumulative number of people with at least one dose.<td>
 		<td>Cumulative fully vaccinated. Cumulative number of fully vaccinated people up to that date.<td>
		<td>Cumulative Johnson & Johnson doses administered up to that date.<td>
<td>N/A<td>
		<td>Cumulative number of vaccines administered up to a particular administration date, includes both single and two-dose series.<td>
	</tr>
	<tr>
		<td>Colorado<td>
		<td>Total given only: people immunized with one dose<td>
 		<td>Totals given only (no county level): people fully immunized <td>
		<td>Totals given only (no county level) <td>
<td>People with additional dose (no county level)<td>
		<td>Total doses administered<td>
	</tr>
	<tr>
		<td>Connecticut<td>
		<td>At least one dose: one dose of any vaccine<td>
 		<td>Fully vaccinated: 2 doses of the Pfizer or Modern vaccines or 1 dose of the J&J. The fully vaccinated are a sunset of the number who have received at least one dose.<td>
		<td>N/A<td>
<td>N/A<td>
		<td>The number of “at least one dose” and “fully vaccinated” add up to more than the number of total doses because people who received the J&J vaccine fit into both categories.<td>
	</tr>
	<tr>
		<td>Delaware<td>
		<td>Total Persons with only 1 Dose of 2-Dose Series<td>
 		<td>Total Persons with 2 Doses of 2-Dose Series <td>
		<td>Total Persons with 1 Dose of 1-Dose Series <td>
<td>Booster/additional doses include additional doses administered after August 13, 2021, to persons who are immunocompromised or as a booster dose to non-immunocompromised persons to increase protection.<td>
		<td>Total Doses Administered - 4/1/2021<td>
	</tr>
	<tr>
		<td>District of Columbia<td>
		<td>The number of COVID-19 Vaccine who have either partially or fully completed the vaccine regimen for COVID-19<td>
 		<td>The number of COVID-19 Vaccine who have completed the vaccine regimen for COVID-19.<td>
		<td>N/A<td>
<td>N/A<td>
		<td>the total number of all administered vaccine<td>
	</tr>
	<tr>
		<td>Florida<td>
		<td>First dose: current number of people who have only received their first dose of the Moderna or Pfizer vaccine.<td>
 		<td>Series Completed: current number of people who have received both Moderna or Pfizer vaccine doses or one Johnson & Johnson dose and are considered fully immunized.<td>
		<td>Completed 1 dose series<td>
<td>Current number of people who have received an additional dose of Pfizer-BioNTech COVID-19 vaccine or Moderna COVID-19
vaccine<td>
		<td>First dose + series complete = Total people vaccinated<td>
	</tr>
	<tr>
		<td>Georgia<td>
		<td>At Least One Dose: Number of residents that have had one or more doses of vaccine<td>
 		<td>Fully Vaccinated: Number of residents that have completed the vaccine series (this may be one or two vaccines depending on the manufacturer)<td>
		<td>N/A<td>
<td>N/A<td>
		<td># Administered<td>
	</tr>
	<tr>
		<td>Hawaii<td>
		<td>Initiating - persons who have received a single dose of any vaccine 4/3/21<td>
 		<td>Completing - persons who have received two doses of the Pfizer or Moderna vaccine or a single dose of the Johnson & Johnson vaccine<td>
		<td>N/A<td>
<td>3rd doses administered<td>
		<td>Total vaccines administered<td>
	</tr>
	<tr>
		<td>Idaho<td>
		<td>received one dose of a two dose series<td>
 		<td>"fully vaccinated"-received single dose of singe series OR two doses of a two dose series<td>
		<td>N/A<td>
<td>N/A<td>
		<td>Vaccinated persons/total persons vaccinated<td>
	</tr>
	<tr>
		<td>Illinois<td>
		<td>Determined by taking the total administered minus the total fully vaccinated<td>
 		<td>Reports total fully vaccinated<td>
		<td>N/A<td>
<td>N/A<td>
		<td>Total Administered Doses – This is the total number of doses (i.e. shots in arms) that have been reported to IDPH.<td>
	</tr>
	<tr>
		<td>Indiana<td>
		<td>Initial dose of 2-series vaccine<td>
 		<td>2nd dose of 2-series vaccine administered<td>
		<td>single dose vaccines administered<td>
<td>”Booster dose” count shows how many booster doses were administered, includes additional COVID-19 vaccinations that were administered at least 27 days after full vaccination<td>
		<td>Total doses administered<td>
	</tr>
	<tr>
		<td>Iowa<td>
		<td>"two dose series initiated"<td>
 		<td>"two dose series completed"<td>
		<td>"single dose series completed"<td>
<td>N/A<td>
		<td>"total doses administered"<td>
	</tr>
	<tr>
		<td>Kansas<td>
		<td>Percent of Kansas Vaccinated: Represents the number of people with at least one dose of a COVID-19 vaccine reported in KS WebIZ as a fraction of the total population of Kansas OR Kansans Vaccinated with One Dose<td>
 		<td>Kansans Completed COVID-19 Vaccine Series<td>
		<td>N/A<td>
<td>3rd dose administered<td>
		<td>Represents the total number of all COVID-19 vaccine doses that have been given to people in Kansas as reported by KS WebIZ<td>
	</tr>
	<tr>
		<td>Kentucky<td>
		<td>N/A<td>
 		<td>N/A<td>
		<td>N/A<td>
<td>N/A<td>
		<td>Total Population Vaccinated <td>
	</tr>
	<tr>
		<td>Louisiana<td>
		<td>Initiated vaccine series, includes of any type of vaccine dose<td>
 		<td>completed the 2 vaccine doses series, including the completion of any vaccine with full completion of vaccine series.<td>
		<td>N/A<td>
<td>N/A<td>
		<td>Determined by summing first and second dose<td>
	</tr>
	<tr>
		<td>Maine<td>
		<td>People who have received the first dose of a COVID-19 vaccine series from Pfizer or Moderna.<td>
 		<td>These are fully vaccinated individuals, who have either received the second dose of the Pfizer or Moderna vaccine, or one dose of the Johnson & Johnson vaccine.<td>
		<td>N/A<td>
<td>Additional/Booster Dose<td>
		<td>Total vaccine doses administered to individuals.<td>
	</tr>
	<tr>
		<td>Maryland<td>
		<td>Number 1st Dose Administered <td>
 		<td>Number 2nd Dose Administered<td>
		<td>Number Single Dose Administered<td>
<td>Additional doses data includes data for individuals who received two initial doses of the same vaccine as part of a two-dose vaccine regimen and received an additional dose of the same vaccine type 28 days or more after the second dose of their initial two-dose vaccine regimen, as identified through Immunet.<td>
		<td>Total Number of Doses Administered<td>
	</tr>
	<tr>
		<td>Massachusetts<td>
		<td>People who have received the first dose of a two series vaccine series, Pfizer or Moderna.<td>
 		<td>Second dose of a two series vaccination series. After second dose a person results in being fully vaccinated.<td>
		<td>receiving the only dose in a single dose vaccine .J&J/Janssen<td>
<td>Booster doses administered: Data on booster doses administered reflect the additional dose recommended after a primary vaccine series<td>
		<td>combination of first and second dose received.<td>
	</tr>
	<tr>
		<td>Michigan<td>
		<td>"Initiation" is the percentage of Michigan residents who have received either 1 or more doses of ANY vaccine.<td>
 		<td>"Completion" is the percentage of Michigan residents receiving 2 doses of Pfizer or Moderna or 1 dose of J&J.<td>
		<td>COVID Vaccine Doses Administered by Vaccine Type --> J&J<td>
<td>Additional doses administered after a primary vaccine series<td>
		<td>"Number of doses administered"" is the number of COVID-19 vaccine doses reported.<td>
	</tr>
	<tr>
		<td>Minnesota<td>
		<td>People with at least one vaccine dose: Number of people in Minnesota who have received either a first or second dose of any COVID-19 vaccine.<td>
 		<td>People with completed vaccine series: Number of people in Minnesota who have completed a COVID-19 vaccine series. For the Pfizer and Moderna products, a complete series is two doses. The Johnson & Johnson product is a single-dose vaccine.<td>
		<td>N/A<td>
<td>Additional doses administered after a primary vaccine series reported at the state level<td>
		<td>Total vaccine doses administered: Number of vaccine doses that have been administered to Minnesotans and reported to the Minnesota Immunization Information Connection (MIIC).<td>
	</tr>
	<tr>
		<td>Mississippi<td>
		<td>One dose of Pfizer/Moderna or one dose of Janssen (Johnson and Johnson) vaccine<td>
 		<td>Second dose of Pfizer/Moderna or one dose of Janssen (Johnson and Johnson) vaccine<td>
		<td>N/A<td>
<td>People Receiving Booster Dose of Pfizer or 3rd Dose of Pfizer or Moderna for Immunocompromising Conditions<td>
		<td>Total doses administered<td>
	</tr>
	<tr>
		<td>Missouri<td>
		<td>People who have received at least one dose<td>
 		<td>People who have completed vaccination<td>
		<td>N/A<td>
<td>3rd doses administered after a primary vaccine series<td>
		<td>Total doses administered<td>
	</tr>
	<tr>
		<td>Montana<td>
		<td>"Dose #1 Administered" - Number of first doses of COVID-19 (for vaccines that are part of a two dose series)<td>
 		<td>Total Montanans Fully Immunized: Total people in Montana that have been fully immunized with the number of doses specific to vaccine manufacturer and ACIP recommendations<td>
		<td>N/A<td>
<td>N/A<td>
		<td>"Total Doses Administered" – Number of COVID-19 vaccine doses administered. This includes Dose 1 and Dose 2.<td>
	</tr>
	<tr>
		<td>Nebraska<td>
		<td>Includes all 1st dose and single dose vaccines administered for Nebraska residents; including those that initiated vaccination in another state. Separated by those given using the Nebraska DHHS allotment and those given using the FVP allotment.<td>
 		<td>The number of Nebraska residents that received the 2nd dose of a vaccine (for those vaccines that require a 2nd dose); includes those that received 2nd doses in another state. Separated by those given using the Nebraska DHHS allotment and those given using the FVP allotment.<td>
		<td>N/A<td>
<td>N/A<td>
		<td>The number of vaccinations given at a Nebraska location includes Nebraska residents and Non-Nebraska residents that received a vaccination at a Nebraska location. This number includes 1st dose (includes 1st dose and single dose) and 2nd doses administered by Nebraska DHHS and FVP providers.<td>
	</tr>
	<tr>
		<td>Nevada<td>
		<td>"Total Vaccinations Reported as Initiated" represents the total number of individuals who have at least initiated a vaccine (anone with a single dose vaccine or the first dose of a two-dose series is included). This is a count of unique individuals who have initiated vaccination, at a minimum. It also includes all who have completed their vaccine series<td>
 		<td>"Total Vaccinations Reported as Completed" represents the total number of individuals who have completed vaccination, whether it is a two-dose series or single dose vaccine. This is also a count of unique individuals, and is a subset of the individuals who are included in initiated<td>
		<td>N/A<td>
<td>N/A<td>
		<td>"Total Doses Reported as Administered" represents the total number of vaccine doses reported as administered, so if an individual has received more than one dose as part of a two dose series that are counted twice<td>
	</tr>
	<tr>
		<td>New Hampshire<td>
		<td>Total dose number 1: received 1 dose of a 2 dose series<td>
 		<td>to be fully vaccinated individuals need to receive 2 doses of Covid 19 vaccination.<td>
		<td>N/A<td>
<td>N/A<td>
		<td>Total doses reported as administered, includes 1st and 2nd doses. <td>
	</tr>
	<tr>
		<td>New Jersey<td>
		<td>Individuals who have received a single dose from a one-dose vaccine course, e.g., the Johnson & Johnson vaccine, or their first dose from a two-dose vaccine course.<td>
 		<td>"fully vaccinated:" Individuals who have received a single dose from a one-dose vaccine course, e.g., the Johnson & Johnson vaccine, or their second dose from a two-dose vaccine course<td>
		<td> Individuals who have received a single dose from a one-dose vaccine course, e.g., the Johnson & Johnson vaccine, or their first dose from a two-dose vaccine course <td>
<td>N/A<td>
		<td>Total vaccine doses administered includes dose 1, dose 2 and a small number of doses that do not have a dose number yet indicated at the time of data refresh. Therefore, summing across dose 1 and dose 2 will not exactly match the total vaccine administered.<td>
	</tr>
	<tr>
		<td>New Mexico<td>
		<td>Number Of New Mexicans With At Least One Shot<td>
 		<td>Number Of New Mexicans Fully Vaccinated<td>
		<td>N/A<td>
<td>Number Of New Mexicans 18+ With A Booster Shot<td>
		<td>Total Doses Administered<td>
	</tr>
	<tr>
		<td>New York<td>
		<td>People with at least one vaccine dose represents the total number of individuals who have received at least one dose of any COVID-19 vaccine.<td>
 		<td>People with completed vaccine series represents the total number of individuals who have completed the recommended series of a given COVID-19 vaccine product.<td>
		<td>N/A<td>
<td>N/A<td>
		<td>Total doses administered represents the total number of vaccine shots, both 1st and 2nd doses, administered to individuals.<td>
	</tr>
	<tr>
		<td>North Carolina<td>
		<td>all first doses of 2 dose series & single dose series<td>
 		<td>all second doses of 2 dose series<td>
		<td>N/A<td>
<td>N/A<td>
		<td>first doses, second doses, & single doses<td>
	</tr>
	<tr>
		<td>North Dakota<td>
		<td>"1 dose coverage rate"<td>
 		<td>"Up-to-Date Coverage Rate"<td>
		<td>N/A<td>
<td>N/A<td>
		<td>"Up-to-Date Coverage Rate"<td>
	</tr>
	<tr>
		<td>Ohio<td>
		<td>“Vaccination started” indicates that the individual has received at least one valid dose of COVID-19 vaccine <td>
 		<td>"“vaccination completed” is a subset of the number included in “vaccination started,” indicating that those individuals within that group have received all recommended COVID-19 vaccine doses 
 and are considered fully immunized"<td>
		<td>N/A<td>
<td>The number of fully vaccinated people (from Vaccine Completed) who received an additional dose of any COVID-19 vaccine on or after August 13, 2021<td>
		<td>the number of individuals that have started and completed the COVID-19 vaccination series by various demographics and county of residence<td>
	</tr>
	<tr>
		<td>Oklahoma<td>
		<td>People with at least one dose. *includes individual count for J&J, Moderna, and Pfizer*<td>
 		<td>completed series of 2 vaccine doses series<td>
		<td>single dose of J&J completion. mixed with prime dose given.<td>
<td>3rd/booster doses administered after completion of a primary series<td>
		<td>Reflects the CDC tracker of administered vaccines. Reported by state, pharmacies, and federal entities.<td>
	</tr>
	<tr>
		<td>Oregon<td>
		<td>Series in progress: in progress to complete their vaccination series <td>
 		<td>Series completed: completed their vaccination series<td>
		<td>Number of Johnson and Johnson doses administered<td>
<td>N/A<td>
		<td>Doses administered by day: total number of COVID19 vaccination doses that have been given to residents <td>
	</tr>
	<tr>
		<td>Pennsylvania<td>
		<td>"Partially Covered" means that the person has received at least one COVID-19 vaccine but has not yet received the necessary number of vaccines at the recommended time intervals to be Fully  Covered. At present, all COVID-19 vaccines under EUA require two doses. As such, an individual partially covered has only received one dose in the two-dose series.<td>
 		<td>"Fully Covered" means that the person has received the necessary number of COVID-19 vaccines at the recommended time intervals.<td>
		<td>N/A<td>
<td>Additional doses administered since August 13, 2021 includes additional doses of mRNA COVID vaccine administered on or after 08-13-2021 to immunocompromised individuals at the CDC recommended interval, as well as booster doses administered to the suggested groups at the recommended intervals, per CDC recommendations<td>
		<td>Total vaccinations administered<td>
	</tr>
	<tr>
		<td>Puerto Rico<td>
		<td>Personas con al mesos una dois (People with at least one dose) *includes individual count for J&J, Moderna, and Pfizer*<td>
 		<td>Personas con serie de vacunas completadas (People with completed vaccine series)<td>
		<td>Total number of J&J doses administered<td>
<td>N.A<td>
		<td>Dosis administradas (Administered doses). Total vaccine doses administered - includes 1st and 2nd doses.<td>
	</tr>
	<tr>
		<td>Rhode Island<td>
		<td>Partially vaccinated: one dose of the Pfizer or Moderna vaccine<td>
 		<td>Number of people fully vaccinated received both doses of either Pfizer or Moderna, or the single-dose Johnson & Johnson vaccine.<td>
		<td>N/A<td>
<td>N/A<td>
		<td>Total doses administered<td>
	</tr>
	<tr>
		<td>South Carolina<td>
		<td>"Total SC Residents with at least 1 Vaccine"<td>
 		<td>"Total SC Residents who have Completed"<td>
		<td>Total Janssen doses given<td>
<td>N/A<td>
		<td>"Total Doses Received by SC Residents" is defined as any individual who received 1 or 2 doses within the state of South Carolina<td>
	</tr>
	<tr>
		<td>South Dakota<td>
		<td># of persons (1 dose)<td>
 		<td># of persons (2 dose)<td>
		<td># of persons administered Janssen<td>
<td>N/A<td>
		<td>Total Doses Administered<td>
	</tr>
	<tr>
		<td>Tennessee<td>
		<td>% county pop. with series initiation (1 dose of Pfizer/Moderna)<td>
<td>% county pop. with series completion; (2 doses of Pfixer/Moderna OR 1 dose of J&J) <td>
		<td>N/A<td>
		<td>N/A<td>
<td>Total doses administered<td>
	</tr>
	<tr>
		<td>Texas<td>
<td>Number of people vaccinated with one dose is defined as the number of people who have received at least one dose of COVID-19 vaccine.<td>
<td>Number of people fully vaccinated is defined as the number of people who have completed the full series (2 doses of Moderna or Pfizer or 1 dose of Janssen vaccine), as outlined by the CDC's Advisory Committee on Immunization Practices (ACIP).<td>
		<td>N/A<td>
<td>N/A<td>
<td>The number of vaccine doses administered, number of people vaccinated with one dose and number of people fully vaccinated are aggregated by the recipient’s county of residence in the first worksheet.<td>
	</tr>
	<tr>
		<td>Utah<td>
		<td>People received at least one dose: anyone who has received one or more doses of a two dose vaccine, like Moderna or Pfizer, or a one dose  vaccine like Johnson and Johnson. This represents all people in Utah whether they are fully vaccinated or partially vaccinated <td>
 		<td>People fully vaccinated: anyone who has completed their vaccine series, either two doses of a two dose vaccine like Pfizer or Moderna, or one dose of a single dose vaccine like Johnson and Johnson. <td>
		<td>N/A<td>
<td>N/A<td>
		<td>Total vaccine doses administered<td>
	</tr>
	<tr>
		<td>Vermont<td>
		<td>Total people started indicates the number of people who have only received the first dose of a two-dose vaccine (Moderna or Pfizer).<td>
 		<td>Total people completed indicates the number of people who completed all doses of the vaccine required (i.e., one for Johnson & Johnson and two for Moderna or Pfizer).<td>
		<td>N/A<td>
<td>N/A<td>
		<td>Doses administered reflects the total number of doses that have been given to people in Vermont, or were reported to Vermont.<td>
	</tr>
	<tr>
		<td>Virginia<td>
<td>"first dose:" Total number of people who received at least one dose of a COVID-19 vaccine, including those who received one dose of the one-dose Johnson & Johnson’s Janssen (J&J) COVID-19 vaccine. This metric includes all people who have received only one dose and those who received at least one dose.<td>
 <td>"fully vaccinated:" Total number of people who have completed the recommended series of a given vaccine product (i.e., two doses of the two-dose Pfizer or Moderna COVID-19 vaccine or one dose of the one-dose Johnson & Johnson’s Janssen (J&J) COVID-19 vaccine).<td>
		<td>*same as first dose<td>
<td>People vaccinated with a booster or third dose after the primary vaccine series, including doses administered through the Federal CDC Pharmacy Partnership. Doses on the Federal Doses Administered dashboard are not included.<td>
<td>This number represents the total doses administered to individuals in Virginia, regardless of whether it was a first dose or a second dose. This number will be greater than the number of individuals who have received at least one dose because some people will have received more than one dose.<td>
	</tr>
	<tr>
		<td>Washington<td>
<td>People initiating vaccination (Receiving at least one dose) *includes people given one dose of any type of vaccine<td>
 <td>People fully vaccinated (Completed recommended number of doses) *People who are fully vaccinated are included in the count of both people initiating vacc. & people fully vaccinated<td>
		<td>N/A<td>
		<td>N/A<td>
<td>Vaccine doses given<td>
	</tr>
	<tr>
		<td>West Virginia<td>
<td>People with At Least One Dose. Represents the people who received at least one dose of Pfizer or Moderna COVID-19 vaccine and includes those who received one dose of the single-shot Johnson and Johnson's Janssen COVID-19 vaccine. This metric includes everyone who has received only one dose and those who received more than one dose.<td>
<td>People who Are Fully Vaccinated: represents the number of people who have received the second dose of Pfizer or Modern COVID-19 vaccine or one dose of the single-shot Johns and Johnson's Janssen COVID-19 vaccine.<td>
		<td>N/A<td>
<td>N/A<td>
<td>The total number of vaccine doses that have been given to people in West Virginia. Includes doses administered at the state level and doses administered through federal programs that includes retail pharmacy and Federal Qualified Health Center.<td>
	</tr>
	<tr>
		<td>Wisconsin<td>
<td>"Residents who have received at least one dose"<td>
 <td>"residents who have completed the vaccine series"<td>
		<td>J&J doses administered<td>
<td>N/A<td>
<td>Total vaccine doses administered: The cumulative number of COVID-19 vaccines administered<td>
	</tr>
	<tr>
		<td>Wyoming<td>
<td>First dose administered (%) Pfizer and Moderna<td>
<td>Second dose administered (%) Pfizer and Moderna<td>
		<td>Doses administered Janssen<td>
<td>N/A<td>
		<td>Total of 1st, 2nd, and Janssen doses administered<td>
	</tr>
</table>
 
# Methodology
Beginning on March 29, 2021, a team of approximately 12 volunteers from the BroadStreet team began tracking vaccine data. At the start of collection, the focus was on archiving data from 18 state dashboards that updated daily and overwrote their data within a 24-hour period. This data was saved in a shared google folder to be entered into spreadsheets at a later date. As capacity grew, states were slowly shifted to data entry. Due to the fact that data was being archived in the beginning of data collection, the dataset is not fully complete and any data prior to when official entry on a given state began is currently filled in with dashes in the dataset. Those entries will be updated as that data is retroactively filled in and included in future releases. 

## Data Limitations
There were various stages in which data collection began for each state within our dataset, as the vaccine team grew. At the start, the focus was just on archiving as much data as possible and that data was saved in shared google folders for later entry. Data collection began with 18 states out of 52, including DC and Puerto Rico. In May, data collection on the remaining states and DC and Puerto Rico began. Due to the inability to collect all data from the beginning, there are gaps present in the dataset. Some states provide historical data on their dashboards, allowing for some gaps to be filled. However, others do not, and that data is no longer recoverable. Within the dataset, dashes are inputted for any states where data was not collected on those dates. If any archived data or historical data exists, those gaps will be filled in retroactively. The table below provides a more in-depth view of when data collection began for each state and whether any historical data exists for that state. 

Table 2. Data Collection by State
 <table>
	<tr>
		<th>State<th>
		<th>Date Entry Began<th>
		<th>Historical Data/Archives<th>
	</tr>
	<tr>
		<td>Alabama<td>
<td>5/14/21<td>
<td>Yes, state level data from 2/10 to 3/16<td>
	</tr>
<tr>
		<td>Alaska<td>
<td>5/13/21<td>
<td>No<td>
	</tr>
<tr>
		<td>Arizona<td>
<td>5/12/21<td>
<td>Yes, just total doses<td>
	</tr>
<tr>
		<td>Arkansas<td>
<td>5/13/21<td>
<td>No<td>
	</tr>
<tr>
		<td>California<td>
<td>4/1/21<td>
<td>Yes, from 12/15/20<td>
	</tr>
<tr>
		<td>Colorado<td>
<td>5/10/21<td>
<td>Yes, 1/9/21<td>
	</tr>
<tr>
		<td>Connecticut<td>
<td>4/29/21<td>
<td>Yes, data by week<td>
	</tr>
<tr>
		<td>District of Columbia<td>
<td>5/15/21<td>
<td>Yes, archives from 3/19<td>
	</tr>
<tr>
		<td>Delaware<td>
<td>5/13/21<td>
<td>Yes<td>
	</tr>
<tr>
		<td>Florida<td>
<td>5/12/21<td>
<td>No<td>
	</tr>
<tr>
		<td>Georgia<td>
<td>5/12/21<td>
<td>Yes<td>
	</tr>
<tr>
		<td>Hawaii<td>
<td>5/14/21<td>
<td>Yes<td>
	</tr>
<tr>
		<td>Idaho<td>
<td>5/13/21<td>
<td>Yes, archived from 3/23<td>
	</tr>
<tr>
		<td>Illinois<td>
<td>5/13/21<td>
<td>No<td>
	</tr>
<tr>
		<td>Indiana<td>
<td>4/1/21<td>
<td>Yes, archived from 3/23<td>
	</tr>
<tr>
		<td>Iowa<td>
<td>4/5/21<td>
<td>Yes, archived from 3/22<td>
	</tr>
<tr>
		<td>Kansas<td>
<td>5/14/21<td>
<td>No<td>
	</tr>
<tr>
		<td>Kentucky<td>
<td>5/14/21<td>
<td>No<td>
	</tr>
<tr>
		<td>Louisiana<td>
<td>5/13/21<td>
<td>No<td>
	</tr>
<tr>
		<td>Maine<td>
<td>4/4/21<td>
<td>3/23/21<td>
	</tr>
<tr>
		<td>Maryland<td>
<td>5/15/21<td>
<td>No<td>
	</tr>
<tr>
		<td>Massachusetts<td>
<td>5/14/21<td>
<td>Yes<td>
	</tr>
<tr>
		<td>Michigan<td>
<td>5/13/21<td>
<td>Yes<td>
	</tr>
<tr>
		<td>Minnesota<td>
<td>4/10/21<td>
<td>No<td>
	</tr>
<tr>
		<td>Mississippi<td>
<td>5/12/21<td>
<td>Yes, archived from 3/23<td>
	</tr>
<tr>
		<td>Missouri<td>
<td>5/14/21<td>
<td>Yes, archived from 3/22<td>
	</tr>
<tr>
		<td>Montana<td>
<td>4/5/21<td>
<td>Yes, archived from 3/22<td>
	</tr>
<tr>
		<td>Nebraska<td>
<td>5/14/21<td>
<td>No<td>
	</tr>
<tr>
		<td>Nevada<td>
<td>5/16/21<td>
<td>No<td>
	</tr>
<tr>
		<td>New Hampshire<td>
<td>5/13/21<td>
<td>Yes<td>
	</tr>
<tr>
		<td>New Jersey<td>
<td>4/5/21<td>
<td>Yes, archived from 3/22/21<td>
	</tr>
<tr>
		<td>New Mexico<td>
<td>4/29/21<td>
<td>Yes, archived from 3/22/21<td>
	</tr>
<tr>
		<td>New York<td>
<td>4/3/21<td>
<td>No<td>
	</tr>
<tr>
		<td>North Carolina<td>
<td>4/12/21<td>
<td>Yes, archived from 3/23/21<td>
	</tr>
<tr>
		<td>North Dakota<td>
<td>5/13/21<td>
<td>Yes, archived from 3/22/21<td>
	</tr>
<tr>
		<td>Ohio<td>
<td>5/13/21<td>
<td>Yes<td>
	</tr>
<tr>
		<td>Oklahoma<td>
<td>5/13/21<td>
<td>No<td>
	</tr>
<tr>
		<td>Oregon<td>
<td>5/9/21<td>
<td>No<td>
	</tr>
<tr>
		<td>Pennsylvania<td>
<td>4/29/21<td>
<td>Yes<td>
	</tr>
<tr>
		<td>Puerto Rico<td>
<td>TBD, issues with data collection, data not included in this release<td>
<td>No<td>
	</tr>
<tr>
		<td>Rhode Island<td>
<td>5/13/21<td>
<td>Yes<td>
	</tr>
<tr>
		<td>South Carolina<td>
<td>4/17/21<td>
<td>Yes, archives from 3/22/21<td>
	</tr>
<tr>
		<td>South Dakota<td>
<td>4/5/21<td>
<td>Yes, archives from 3/22/21<td>
	</tr>
<tr>
		<td>Tennessee<td>
<td>4/29/21<td>
<td>Yes, archives from 3/22/21<td>
	</tr>
<tr>
		<td>Texas<td>
<td>4/5/21<td>
<td>Yes, archives from 3/22/21<td>
	</tr>
<tr>
		<td>Utah<td>
<td>5/15/21<td>
<td>Yes<td>
	</tr>
<tr>
		<td>Vermont<td>
<td>5/13/21<td>
<td>Yes<td>
	</tr>
<tr>
		<td>Virginia<td>
<td>4/12/21<td>
<td>Yes<td>
	</tr>
<tr>
		<td>Washington<td>
<td>5/10/21<td>
<td>No<td>
	</tr>
<tr>
		<td>West Virginia<td>
<td>5/13/21<td>
<td>No<td>
	</tr>
<tr>
		<td>Wisconsin<td>
<td>5/15/21<td>
<td>No<td>
	</tr>
<tr>
		<td>Wyoming<td>
<td>4/5/21<td>
<td>Yes, archives from 3/23/21<td>
	</tr>
</table>

## Data Entry
Each day, data entry team members enter data from state or county health departments onto a shared google sheet. To limit errors, each state had its own tab with counties and variables listed for each day. At the top of each day, there is a row for calculated totals which is determined from the sum of county entries and a row for reported state totals, the numbers of which should be the same. After entering in data for a given day, interns would then check to make sure those numbers equated to each other, and if they didn’t, they reviewed their entry for errors. If no errors were found, Project Leads were notified of the discrepancy for further investigation. In multiple instances it was found that those numbers did not always result in the same value and very rarely was there any indication on the dashboard as to why that may be the case. After entry was completed, the Project Leads would then do a first check to ensure data was filled in completely, and matched reported state totals. Cumulative totals should, by definition, be constantly trending upwards. In any instance where the totals decreased from the previous day, we investigated the cause of the revision and corrected historic data accordingly. Health departments frequently do not report the information needed to correct these “trend breaks.” In some instances, health departments move individuals out of the “1st Dose” category when they receive their “2nd Dose” or are Fully Vaccinated (they have completed a full series of either a two-dose series or 1-dose of a single dose series), which results in a decrease in 1st Dose numbers between days.

## Data Source
Interns collect data from health department sites at the state level. Currently, the states where data entry is occurring have data available at the county-level on a centralized state dashboard. As more states are added, the need for health department sites at the county-level will be assessed and added to the data sources. 

## Data Collection & Input
Data is collected every day for all 50 states, plus DC and Puerto Rico. Some still report data at just the state-level, so county-level data is not yet determinable for all states. 

Data is collected as cumulative doses rather than new daily doses. Both unknown and out-of-state administration of vaccines are also recorded if available and listed on the dashboard. Any doses that are not linked to a specific county or are not explicitly stated as out-of-state, are recorded in the unknown category. 
When counties report data as a percentage, the percentage for each variable is multiplied by the total number of doses administered to determine the raw data, unless otherwise stated on the dashboard (some report as % of county population rather than % of total doses). 

## Missing Data
Intermittently, volunteers miss recording data from states that regularly overwrite the data on their state dashboard. Since there is no comparison set for use and, in almost all cases, historical data is not present, the current protocol is to copy over the data from the last completed day to fill in the gaps.. Systems are being implemented to prevent this in the future. In the event that those systems are insufficient in capturing the data or fail to provide a complete data set, data from the most recent day will continue to be carried over.  

# Data Challenges

## Changes in Process
During early months, we found that most states were reporting single dose vaccines with either first dose or second dose numbers. Slowly as the J&J vaccine became more widely used, states started separating out single dose vaccines and reporting them separately. As those changes occurred, we corrected our reporting to follow suit and edited definitions as needed. 

On March 27th, 2021, Indiana started reporting single doses for vaccines separately at the county level. We started recording single dose vaccinations for the state. 
Prior to April 14th, 2021, as a result of the way Indiana displays its data, some interns were reporting the number for fully vaccinated in the total doses column, which only included second dose and single dose numbers. This was corrected on April 14th to reflect the number of total doses administered, prior to this some discrepancies in the number of total doses is present and was noted on the spreadsheet. 

On April 14th, 2021, we began separating Janssen (J&J) vaccines from the “Number of People of Initiating Vaccine Series'', allowing for single doses to be captured separately from 1st doses of Moderna and Pfizer vaccines administered for South Dakota. Prior to this, single dose counts were being included in the first dose counts due to the way the data was displayed. 

On April 23rd, 2021, New Jersey began reporting total Janssen doses administered at the state level. 

On July 30th, 2021 the Tennessee dashboard was updated to capture single dose vaccination numbers and began reporting them as percentages. We began recording single dose vaccination numbers for the state, at both the state and county levels. 

### Reporting Changes
On May 5th, 2021, it was noted that Chicago County, Illinois was missing from the data entry sheet and was added at that time. Prior to this, any data for this county was missed. 

On June 8th, 2021, the state of Florida changed its reporting for daily to a single weekly report and no longer provided a separate report for detailed county information. This change in reporting resulted in only total dosage administration being reported at the county-level. From this day forward to present day, 1st, 2nd, and single dose information at the county-level is filled in with a dash to reflect the stop in reporting by the Florida Health Department.

On June 25th, 2021, the state of Arkansas began displaying information for 1st and 2nd doses at the county-level. Previously only 2nd dose information was available, which was also recorded in the total dose column in the dataset. When the additional data became available, the reporting in the dataset was adjusted to reflect the new information. 
 
On July 2nd, 2021 the Nebraska dashboard was no longer accessible. Their Health Department website had a message stating that “The State of Nebraska COVID-19 Dashboard is no longer available as of June 30, 2021. Any future updates regarding coronavirus will be provided through new releases and through other means.” On July 20th, 2021 two new resources for vaccine information for the state of Nebraska were found. The first, provided by the state of Nebraska Health Department in response to a query submitted about accessibility of data, only updates state-level information on a weekly basis. The second resource allowed for the addition of county-level total dose information to be recorded. Beginning July 23rd, 2021 these resources were implemented into data entry and dose information began to be recorded again. Data from June 30-July 22, 2021 was copied down until the new resources were available. 

On August 13th, 2021 a change was made in the entry of “totals doses” administered for Puerto Rico. Prior to 8/13/2021, the totals, at the municipality level, were being determined by summing the three variables reported to obtain a number for total doses. Based on the way the dashboard data was displayed, it was found that “single doses” for Puerto Rico were being double-counted in both the first and second dose reporting levels. This was confirmed when Puerto Rico updated their dashboard and began displaying an “accumulated doses given” graph. The reporting changed to being “1st + 2nd - single” to get the appropriate number of total doses administered at both the state and municipality level.This shift in reporting resulted in a decline in total doses being seen from this day forward compared to those previously reported.  



## Accessibility of Data: Geographic Breakdown
States differ in how they present their data and the geographic breakdowns they provide. Most states report vaccine information at both the state- and county-level, however a handful report only state-level data. In the case where only state-level data is available, the dataset is filled in with zeros for each county and only the state totals row is inputted with numbers. Some states provide geographic breakdowns that are not at the county-level, like Oklahoma, Nebraska, and Utah. Oklahoma only provides a breakdown of vaccine data by zip code. Nebraska only provides vaccine data by health district. Utah provides vaccine data as a mix of jurisdictions and counties. Due to the fact that all the data is not explicitly listed for a single county, this makes it challenging to capture the data accurately at the county-level. Currently in the dataset, unless a county is listed in their reporting, these states only have data inputted for the state totals and zeros inputted for the counties. As some of that data may be able to be translated into county-level information, that will change to reflect that information.   

## Accessibility of Data: Formatting
State websites report data related to the COVID-19 pandemic in various formats, which complicates any efforts to automate data entry. Formats used to report vaccine data include .csv, .pdf, GIS, Microsoft BI, Tableau, and plain text. 

# Suggested Citation
When using data images, downloaded data, or shared document formats, please attribute BroadStreet as well as the original source, when applicable. For examples and more information, review this article which answers the question ["How do I cite BroadStreet?"] (https://help.broadstreet.io/article/citations/)

# Contributors
Tom Schmitt, PhD, Tracy Flood, MD PhD, [Kaiynat Amir, MPH] (https://www.linkedin.com/in/kaiynat-amir), [Rachael Church] (https://www.linkedin.com/in/rchurch20/). A full list of the Broadstreet Covid-19 Data Project volunteers can be found here: <https://covid19dataproject.org/team-2/>
