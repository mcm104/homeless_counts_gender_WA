# Homeless Counts in Washington State by Gender, 2015-2019
_This dataset was created as a final project for the University of Washington Information School's Winter 2021 course on data curation._

This dataset contains the results of point-in-time homelessness counts in Washington state from 2015 to 2019. The counts are broken up by gender and housing status. You will find counts for four gender categories: cisgender female, cisgender male, transgender, and gender non-conforming. In this dataset you will find the counts for all four categories, which are further broken down by current housing status: in an emergency shelter, in transitional housing, or unsheltered. The intended audience for this dataset is policymakers at the municipal, county, and state level in Washington state.

## A note about the language in this dataset
The data from this dataset comes from point-in-time homeless counts conducted by [Continuum of Care (CoC) Homeless Assistance Programs](https://www.hudexchange.info/programs/coc/), who are required to submit the results of these counts to the U.S. Department of Housing and Urban Development (HUD) as part of their CoC membership. Beginning in 2015, the source data provides counts for three gender categories: female, male, and transgender. In 2017, a fourth category was added for gender non-conforming persons.

The gender categories used in this dataset have been revised from the original CoC data. Female, male, and transgender are not mutually exclusive terms; a transgender woman, for example, is both transgender and female. However, these terms are used in the source data as though they were mutually exclusive. The opposite of transgender is cisgender. Therefore, the categories 'female' and 'male' have been renamed to 'cisgender female' and 'cisgender male,' in order to be more precise, to make the labels more in line with the intent of the source data, and to be more respectful of the transgender community. The publisher of this dataset invites researchers using this data to be mindful and respective of trans-inclusive terminology in their research.

# Metadata
_Recorded using [Project Open Data Metadata Schema](https://resources.data.gov/resources/dcat-us/)_
| **Attribute** | **Value** |
| --- | --- |
| **title** | Homeless Counts in Washington State by Gender, 2015-2019 |
| **description** | This dataset contains the results of point-in-time homelessness counts in Washington state from 2015 to 2019. The counts are broken up by gender and housing status. |
| **temporal** | 2015-2019 |
| **accessLevel** | public |
| **issued** | 2021-03-08 |
| **language** | en-us |
| **landingPage** | https://github.com/mcm104/homeless_counts_gender_WA |
| **describedBy** | https://github.com/mcm104/homeless_counts_gender_WA#data-dictionary |
| **publisher** | Melissa Morgan |
| **contactPoint** | Melissa Morgan <mailto:mcm104@uw.edu> |
| **references** | https://files.hudexchange.info/reports/published/CoC_PopSub_State_WA_2015.pdf, https://files.hudexchange.info/reports/published/CoC_PopSub_State_WA_2016.pdf, https://files.hudexchange.info/reports/published/CoC_PopSub_State_WA_2017.pdf, https://files.hudexchange.info/reports/published/CoC_PopSub_State_WA_2018.pdf, https://files.hudexchange.info/reports/published/CoC_PopSub_State_WA_2019.pdf
| **keyword** | homeless, homelessness, washington, washington state, trans, transgender, trans homelessness |
| **theme** | homelessness, gender |
| **identifier** | homeless_counts_gender_WA |

# Data Dictionary

| **Variable** | **Variable name** | **Variable type** | **Allowed values** | **Description** |
| --- | --- | --- | --- | --- |
| **Gender** | gender | Text | cisgender_male, cisgender_female, transgender, GNC | The gender of the given segment of persons in a homeless count. GNC stands for "gender non-conforming" and refers to individuals who do not identify as cisgender male, cisgender female, or transgender. |
| **Year of count** | year | Date/time | 2015-2019 | The year in which the homeless count occurred. |
| **Number of homeless persons living in an emergency shelter** |	num_emergency_shelter |	Number |	0-n	| The number of persons of the given gender who were living in an emergency shelter at the time of the homeless count. |
| **Percentage of homeless persons living in an emergency shelter** |	per_emergency_shelter |	Percentage |	0%-100% |	The percentage of homeless persons of the given gender who are living in an emergency shelter at the time of the homeless count. |
| **Number of homeless persons living in transitional housing** |	num_transitional housing |	Number |	0-n	| The number of persons of the given gender who were living in transitional housing at the time of the homeless count. |
| **Percentage of homeless persons living in transitional housing** |	per_transitional housing |	Percentage |	0%-100% |	The percentage of homeless persons of the given gender who are living in transitional housing at the time of the homeless count. |
| **Number of homeless persons who are unsheltered** |	num_unsheltered	| Number |	0-n |	The number of persons of the given gender who were unsheltered at the time of the homeless count. |
| **Percentage of homeless persons who are unsheltered** |	per_unsheltered	| Percentage |	0%-100% |	The percentage of homeless persons of the given gender who are living in an emergency shelter at the time of the homeless count. |
| **Total number of homeless persons** |	num_total |	Number |	0-n |	The total number of persons of the given gender who were counted during the homeless count. |
