# Data Sheet for Programs
The description of required and recommended fields for programs data follows. Programs data files for upload may include any additional fields not listed here. 

## Required Fields
The outlined fields are required to derive the required set of provider outcomes. Field header names need not exactly match those outlined below in the files uploaded.

Data Field | Description
------ | -----------
**program_provider** | Name of provider offering a training program. This may be a college(2-year or 4-year), vocational institute or organization offering programs
**program_name** | Name of program being offered by the training provider
**program_code** | Numeric code uniquely identifying the category in which program falls, e.g Classification of Instructional Programs(CIP) code for the program
**program_description** | Description of the program offered
**program_status** | Current status of the program, indicating if it is still offered by the training provider e.g `Open`, `Discontinued`, `Deferred`
**program_fees** | Cost of the program offered
**geographic_areas** | Area(s) serviced by the program, this could be state, county or city
**program_address** | Physical address where the program is offered
 **eligibility_criteria** | Requirement(s) for eligibility to enroll for the program e.g `Residents`, `MilitarySpouse`, `BachelorsLevel`. This closely [links to `Audience` and `Audience Level` in Credentials recommended fields](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/datasheets/CREDENTIALS.md#recommended-fields) 
**credential_earned** | Credential earned after completion of the program. This matches the [`credential_type` in the Credentials required fields](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/datasheets/CREDENTIALS.md#required-fields) | 
**program_potential_outcome** | Numeric code(0-9) indicating the potential outcome of the program of study, see the [ETA codes]() for corresponding outcomes

## Recommended Fields
The following fields are not required but they are recommended to provide more insights into program data.

Data Field | Description
------ | -----------
**program_contact_phone** | Phone number for the program's contact
**program_contact_email** | Email address for the program's contact
**program_website** | URL for the program or provider's website
**languages** | Languages in which the program is offered
**current_intake_capacity** | Number of participants that the program can enroll
**program_offering_model** | Also known as the `program format`, a numeric code indicating how is a program offered? Classes at a physical location, online, set of workshops? See the [ETA codes]() for the corresponding offering models. These closely relates to the `learning_method` captured in [Credentials recommended fields](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/datasheets/CREDENTIALS.md#recommended-fields)
**program_length_hours** | Duration of program instruction in hours, typically for short-running programs
**program_length_weeks** | Duration of program instruction in weeks, typically applicable to longer running programs
**pre-requisites** | Numeric code(0-5) indicating pre-requisite training and/or credentials are required to qualify for the program, see the [ETA codes]() for corresponding pre-requisites
**program_soc** | 8-digit O\*NET `Standard Occupational Classification (SOC)` code(without dashes or decimal points) for which this program prepares participant. This has a [mapping to the program CIP code](https://www.onetonline.org/crosswalk/CIP?s=&g=Go)

**funding_sources** | Sources of funding for the program including state or federal support
**is_etpl** | Where applicable, is this program on the Eligible Training Provider List(ETPL)? An indication of `Yes` or `No`, null entry is assumed to be `N/A`

## Data Samples
See what a valid programs file could look like from the [templates](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/templates/programs.csv).
