# trans_homeless_counts_WA

_This dataset was created as a final project for the University of Washington Information School's Winter 2021 course on data curation._

This dataset contains the results of point-in-time homelessness counts in Washington state from 2015 to 2019. The counts are broken up by gender and housing status. The source data provides three gender categories: female, male, and transgender. In 2017, a fourth category was added for gender nonconforming persons. In this dataset you will find the counts for all four categories, as well as counts and percentages within each category for those in emergency shelters, those in transitional housing, and those who are unsheltered. The intended audience for this dataset is policymakers at the municipal, county, and state level in Washington state.

# Metadata

| **Attribute** | **Value** |
| --- | --- |
| **title** | title |
| **description** | description |
| **temporal** | 2015-2019 |
| **accessLevel** | public |
| **issued** | 2021-03-08 |
| **language** | en-us |
| **landingPage** | https://github.com/mcm104/trans_homeless_counts_WA |
| **describedBy** | https://github.com/mcm104/trans_homeless_counts_WA#data-dictionary |
| **publisher** | Melissa Morgan |
| **contactPoint** | Melissa Morgan <mailto:mcm104@uw.edu> |
| | https://files.hudexchange.info/reports/published/CoC_PopSub_State_WA_2015.pdf, https://files.hudexchange.info/reports/published/CoC_PopSub_State_WA_2016.pdf, https://files.hudexchange.info/reports/published/CoC_PopSub_State_WA_2017.pdf, https://files.hudexchange.info/reports/published/CoC_PopSub_State_WA_2018.pdf, https://files.hudexchange.info/reports/published/CoC_PopSub_State_WA_2019.pdf
| **keyword** | homeless, homelessness, washington, washington state, trans, transgender, trans homelessness |
| **identifier** | trans_homeless_counts_WA |

# Data Dictionary

| **Variable** | **Variable name** | **Variable type** | **Allowed values** | **Description** |
| --- | --- | --- | --- | --- |
| **Gender** | gender | Text | male, female, transgender, GNC | The gender that the given segment of persons are identified as in a homeless count.Gender values based on those provided in source data. GNC stands for "gender non-conforming" and refers to individuals who do not identify as male, female, or transgender. |
| **Year of count** | year | Date/time | 2015-2019 | The year in which the homeless count occurred. |
| **Number of homeless persons living in an emergency shelter** |	num_emergency_shelter |	Number |	0-n	| The number of persons of the given gender who were living in an emergency shelter at the time of the homeless count. |
| **Percentage of homeless persons living in an emergency shelter** |	per_emergency_shelter |	Percentage |	0%-100% |	The percentage of homeless persons of the given gender who are living in an emergency shelter at the time of the homeless count. |
| **Number of homeless persons living in transitional housing** |	num_transitional housing |	Number |	0-n	| The number of persons of the given gender who were living in transitional housing at the time of the homeless count. |
| **Percentage of homeless persons living in transitional housing** |	per_transitional housing |	Percentage |	0%-100% |	The percentage of homeless persons of the given gender who are living in transitional housing at the time of the homeless count. |
| **Number of homeless persons who are unsheltered** |	num_unsheltered	| Number |	0-n |	The number of persons of the given gender who were unsheltered at the time of the homeless count. |
| **Percentage of homeless persons who are unsheltered** |	per_unsheltered	| Percentage |	0%-100% |	The percentage of homeless persons of the given gender who are living in an emergency shelter at the time of the homeless count. |
| **Total number of homeless persons** |	num_total |	Number |	0-n |	The total number of persons of the given gender who were counted during the homeless count. |
