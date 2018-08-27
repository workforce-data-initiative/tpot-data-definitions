# Data Sheet for Participants
The description of required and recommended fields for participants data follows. Participants data files for upload may include any additional fields not listed here.

Ideally, participants data should go back approximately two years or more, so that complete outcomes calculations can be produced.

## Required Fields
The outlined fields are required to derive the required set of provider outcomes. Files uploaded need not necessarily use the same field header names.

Data Fields | Description
------------| --------------
**participant_id** | Unique ID identifying a program participant throughout period of participation, e.g a Social Security Number. Participant unique identification supports operations like wage matching for outcomes derivation
**program_code** | Numeric code uniquely identifying the category in which program falls e.g it's Classification of Instructional Programs(CIP). This maps to the [`program_code` in the Programs required fields](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/datasheets/PROGRAMS.md#required-fields)
**program_provider** | Name of provider offering a training program. This may be a college (2-year or 4-year), vocational institute or organization offering programs
**entry_date** | Date participant commenced the program, this may differ from the enrollment date and the official date of program commencement set by the provider, in the format `YYYYMMDD`
**exit_date** | Date participant exited the program, in the format `YYYYMMDD`
**exit_type** | Nature of participant's exit from the program e.g `Graduated`, `Transferred`, `Completed` etc
**exit_reason** | For individuals that exit program based on exit types related to abandonment of program, use any of these numeric values to capture why, `01 = Institutionalized`, `02 = Health/Medical`, `03 = Deceased`, `04 = Reserve Forces called to Active Duty`, `05 = Foster Care`, `06 = Ineligible`, `99 = Not a Valid SSN`, `00 = Other`. There is also an additional option, `98 = Retirement`. These options are based on the WIOA codes provided in [PIRL]() at this time

## Recommended Fields
The following fields are not required but they are recommended to provide additional data for outcomes analysis.

Data Fields | Description
------------| --------------
**program_name** | Name of the participant's program
**service_location** | Geographic location of service of the program a participant is enrolled in. Ideally this would map to one of the [`geographic areas` in the Programs required fields](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/datasheets/PROGRAMS.md#required-fields)
**funding_sources** | Sources of funding for the participant's program. Sources of funding may relate to [`funding sources` captured for Programs data](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/datasheets/PROGRAMS.md#recommended-fields)

## Data Samples
See what a valid participants file could look like from the [templates](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/templates/participants.csv).
