# Data Sheet for Participants
The description of required and recommended fields for participants data follows. Participants data files for upload may include any additional fields not listed here.

## Required Fields
The outlined fields are required to derive the required set of provider outcomes. Files uploaded need not necessarily use the same field header names.

_**TO BE ADDED**: Additional fields for participant wages data_

Data Fields | Description
------------| --------------
**participant_id** | Unique ID identifying a program participant, e.g a Social Security Number. Participant unique identification supports operations like wage matching for outcomes derivation
**wioa_participant** | Indic
**program_code** | Numeric code uniquely identifying the category in which program falls e.g it's Classification of Instructional Programs(CIP). This maps to the [`program_code` in the Programs required fields](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/datasheets/PROGRAMS.md#required-fields)
**entry_date** | Date participant commenced the program, this may differ from the enrollment date and the official date of program commencement set by the provider
**exit_date** | Date participant exited the program
**exit_type** | Nature of participant's exit from the program e.g `Graduated`, `Transferred` etc. This maps to the [`program_potential_outcome` in the Programs required fields](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/datasheets/PROGRAMS.md#required-fields)
**wioa_participant** | Is participant a Workforce Innovation and Opportunity Act(WIOA) beneficiary? An indication of Yes or No, null entry is assumed to be No

## Recommended Fields
The following fields are not required but they are recommended to provide additional data for outcomes analysis.

Data Fields | Description
------------| --------------
**program_name** | Name of the participant's program
**service_location** | Geographic location of service of the program a participant is enrolled in. Ideally this would map to one of the [`geographic areas` in the Programs required fields](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/datasheets/PROGRAMS.md#required-fields)
**funding_sources** | Sources of funding for the participant's program. Sources of funding may relate to [`funding sources` captured for Programs data](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/datasheets/PROGRAMS.md#recommended-fields)

## Data Samples
See what a valid participants file could look like from the [templates](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/templates/participants.csv).
