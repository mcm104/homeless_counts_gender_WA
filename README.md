# Homeless Counts in Washington State by Gender, 2015-2019
_This dataset was created as a final project for the University of Washington Information School's Winter 2021 course on data curation._

This dataset contains the results of point-in-time homelessness counts in Washington state from 2015 to 2019. The counts are broken up by gender and housing status. You will find counts for four gender categories: cisgender female, cisgender male, transgender, and gender non-conforming. In this dataset you will find the counts for all four categories, which are further broken down by current housing status: in an emergency shelter, in transitional housing, or unsheltered. The intended audience for this dataset is policymakers at the municipal, county, and state level in Washington state.

## A note about the language in this dataset
The data from this dataset comes from point-in-time homeless counts conducted by [Continuum of Care (CoC) Homeless Assistance Programs](https://www.hudexchange.info/programs/coc/), who are required to submit the results of these counts to the U.S. Department of Housing and Urban Development (HUD) as part of their CoC membership. Beginning in 2015, the source data provides counts for three gender categories: female, male, and transgender. In 2017, a fourth category was added for gender non-conforming persons.

The gender categories used in this dataset have been revised from the original CoC data. Female, male, and transgender are not mutually exclusive terms; a transgender woman, for example, is both transgender and female. However, these terms are used in the source data as though they were mutually exclusive. The opposite of transgender is cisgender. Therefore, the categories 'female' and 'male' have been renamed to 'cisgender female' and 'cisgender male,' in order to be more precise, to make the labels more in line with the intent of the source data, and to be more respectful of the transgender community. The publisher of this dataset invites researchers using this data to be mindful and respective of trans-inclusive terminology in their research.

## File naming conventions used
File names should use the project abbreviation HCG_WA (homeless counts by gender in Washington) and the file version number. For example...
```
HCG_WA_1.0.1.csv
```
The original data as retrieved from HUB Exchange is in a ZIP file labeled with version number 1.0.0.

Normalized data is stored as a CSV file.

## Data normalization
The following steps have been carried out on the source data in order to create this dataset:
1. Homeless counts broken down by gender manually recorded from multiple CoC reports and placed into a single dataset.
2. Allowed values for the variable "gender" renamed as follows:
   - Female --> **cisgender_female**
   - Male --> **cisgender_male**
   - Do not identify as Female, Male, or Transgender\* --> **GNC**
   - Gender Non-Conforming (i.e. not exclusively male or female) --> **GNC**
3. Rows ordered to keep gender categories together, and chronologically by year within gender categories.
4. Rows added for gender categories that do not have data for every year in the scope of the dataset (namely, rows have been added for 2015 and 2016 for the GNC category).
5. Columns added to record the percentages within each year and gender category that are in each category of housing status.
6. Blank values filled in as "NA".

_*This category was only used once in 2017 before being renamed to Gender Non-Conforming_

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
| **Number of homeless persons living in an emergency shelter** |	number_emergency_shelter |	Number |	0-n	| The number of persons of the given gender who were living in an emergency shelter at the time of the homeless count. |
| **Percentage of homeless persons living in an emergency shelter** |	percent_emergency_shelter |	Percentage |	0%-100% |	The percentage of homeless persons of the given gender who are living in an emergency shelter at the time of the homeless count. |
| **Number of homeless persons living in transitional housing** |	number_transitional housing |	Number |	0-n	| The number of persons of the given gender who were living in transitional housing at the time of the homeless count. |
| **Percentage of homeless persons living in transitional housing** |	percent_transitional housing |	Percentage |	0%-100% |	The percentage of homeless persons of the given gender who are living in transitional housing at the time of the homeless count. |
| **Number of homeless persons who are unsheltered** |	number_unsheltered	| Number |	0-n |	The number of persons of the given gender who were unsheltered at the time of the homeless count. |
| **Percentage of homeless persons who are unsheltered** |	percent_unsheltered	| Percentage |	0%-100% |	The percentage of homeless persons of the given gender who are living in an emergency shelter at the time of the homeless count. |
| **Total number of homeless persons** |	number_total |	Number |	0-n |	The total number of persons of the given gender who were counted during the homeless count. |
