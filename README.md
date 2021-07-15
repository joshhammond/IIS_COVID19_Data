# IIS_COVID19_Data

[![CC BY 4.0][cc-by-shield]][cc-by]

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg


Thomas Hale, Noam Angrist, Rafael Goldszmidt, Beatriz Kira, Anna Petherick, Toby Phillips, Samuel Webster, Emily Cameron-Blake, Laura Hallas, Saptarshi Majumdar, and Helen Tatlow. (2021). “A global panel database of pandemic policies (Oxford COVID-19 Government Response Tracker).” Nature Human Behaviour. https://doi.org/10.1038/s41562-021-01079-8

This data is a modification of data provided by the Oxford Covid-19 Government Response Tracker (OxCGRT) project.  The main webpage for the project is located here:
https://www.bsg.ox.ac.uk/research/research-projects/covid-19-government-response-tracker

The data (which is updated frequently) is located on Git-Hub here:
https://github.com/OxCGRT/covid-policy-tracker


Table 1: Data Dictionary
| Name | Description|	Data | Type |	Example |
| --- | --- | --- | --- | --- |
|CountryName|	Country Name|	String|	United States|
|RegionName|	Sub-National Regions (State, etc.)|	String| |	
|Jurisdiction|	NAT_TOTAL or STATE_TOTAL|	String|	NAT_TOTAL|
|Date|	Reported date|	Date|	3/21/2020|
|C1_SchoolClosing|	Record closings of schools and universities; ordinal scale of 0 to 3|	Integer|	3|
|C2_WorkspaceClosing|	Record closings of workspace; ordinal scale of 0 to 3|	Integer|	3|
|C3_CancelPublicEvents|	Record cancelling public events; ordinal scale of 0 to 2|	Integer|	2|
|C4_RestrictionsGatherings|	Record limits on gatherings; ordinal scale of 0 to 4|	Integer|	4|
|C5_ClosePublicTransport|	Record closings of public transport; ordinal scale of 0 to 2|	Integer|	1|
|C6_StayAtHome|	Record orders to ‘shelter-in-place’; ordinal scale of 0 to 3|	Integer|	2|
|C7_RestrictionsIntMvt|	Record restrictions on internal movement between cities/regions; ordinal scale of 0 to 2|	Integer|	2|
|C8_InternationalTravel|	Record restrictions on international travel; ordinal scale of 0 to 4|	Integer|	3|
|E1_Income support|	Record if cash payments to people who lose jobs; ordinal scale of 0 to 2|	Integer|	0|
|E2_Debt/contract relief|	Record if freezing financial obligations for households; ordinal scale of 0 to 2|	Integer|	0|
|E3_Fiscal measures|	Announced economic stimulus spending|	Float|	0|
|E4_International support|	Announced offers of aid spending to other countries|	Float|	0|
|H1_PublicInfo|	Record of public info campaigns; ordinal scale of 0 to 2|	Integer|	2|
|H2_TestingPolicy|	Record who has access to testing; ordinal scale of 0 to 3|	Integer|	3|
|H3_Contact_Tracing|	Record gov policy on contact tracing after a positive diagnosis; ordinal scale of 0 to 2|	Integer|	1|
|H4_EmergencyHealthcareInvest|	Announced short term spending on healthcare|	Float|	0|
|H5_InvestmentInVaccines|	Announced spending on vaccine development|	Float|	0|
|H6_FacialCoverings|	Record policies on facial coverings outside home; ordinal scale of 0 to 4|	Integer|	1|
|H7_VaccinationPolicy|	Record policies on vaccine delivery for diff groups; ordinal scale of 0 to 5|	Integer|	0|
|C1/C2/C3/C4/C5/C6/C7 E1/H1/H6/H7 Flags|	See OxCGRT documentation for details|	Binary Flag|	0|
|ConfirmedCases|	Cumulative confirmed cases|	Integer|	26025|
|ConfirmedDeaths|	Cumulative confirmed deaths|	Integer|	475|
|StringencyIndex|	C1+C2+C3+C4+C5+C6+C7+C8+H1|	Float|	72.69|
|GovernmenResponseIndex|	C1+C2+C3+C4+C5+C6+C7+C8+H1+H2+H3+H6+H7|	Float|	54.44|
|ContainmentHealthIndex|	C1+C2+C3+C4+C5+C6+C7+C8+H1+H2+H3+H6+H7+E1+E2|	Float|	62.82|
|EconomicSupportIndex|	E1+E2|	Float|	0|
