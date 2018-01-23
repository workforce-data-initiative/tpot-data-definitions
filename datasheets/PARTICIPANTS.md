# Data Sheet for Participants
The description of required and recommended fields for participants data follows. Participants data files for upload may include any additional fields not listed here.

## Required Fields
The outlined fields are required to derive the required set of provider outcomes. Files uploaded need not necessarily use the same field header names.

Data Fields | Description
------------| --------------
**participant_code** | Unique ID identifying a program participant. Participant unique identification will support operations like wage matching for outcomes derivation
**program_code** | Unique ID identifying the participant's program e.g Classification of Instructional Programs(CIP). This would map to the [`program_code` in the Programs required fields](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/datasheets/PROGRAMS.md#required-fields) 
**potential_credential** | Prospective credential that participant can (or has already) obtained from the program they are enrolled in. This closely captures the [`credential_type` in the Credentials required fields](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/datasheets/CREDENTIALS.md#required-fields)
**entry_date** | Date participant commenced the program, this may differ from the enrollment date and the official date of program commencement set by the provider
**exit_date** | Date participant exited the program
**type_of_exit** | Nature of participant's exit from the program e.g `Transfered`, `Completed`, `Withdrawn`, `Suspended`
**obtained_credential** | Did the participant obtain the credential awarded by the provider for the program? An indication of `Yes` or `No`
**participant_funding** | Source of funding for the participant's program


## Recommended Fields
The following fields are not required but they are recommended to provide additional data for outcomes analysis.

Data Fields | Description
------------| --------------
**program_name** | Name of the participant's program
**service_location** | Geographic location of service of the program a participant is enrolled in. Ideally this would map to one of the [`geographic areas` in the Programs required fields](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/datasheets/PROGRAMS.md#required-fields)

## Data Samples
See what a valid participants file could look like from the [templates](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/templates/participants.csv).
