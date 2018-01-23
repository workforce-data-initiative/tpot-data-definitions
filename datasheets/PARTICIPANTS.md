# Data Sheet for Participants
The description of required and recommended fields for participants data follows. Participants data files for upload may include any additional fields not listed here.

## Required Fields
The outlined fields are required to derive the required set of provider outcomes. Files uploaded need not necessarily use the same field header names.

Data Fields | Description
------------| --------------
**participant_code** | Unique ID identifying a program participant. Participant unique identification will support operations like wage matching for outcomes derivation.
**program_code** | Unique ID identifying the participant's program e.g Classification of Instructional Programs(CIP). This would map to the [`program_code` in the Programs required fields](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/datasheets/PROGRAMS.md#required-fields) 
**program_name** | Name of the participant's program
**potential_outcome** | Indication of possible outcomes of the program participant is enrolled in
**date_of_entry** | 
**date_of_exit** |
**type_of_exit** | Nature of participant's exit from the program
**obtained_credential** |
**participant_funding** | Source of funding for the participant's program


<!-- ## Recommended Fields -->
<!-- The following fields are not required but they are recommended to provide additional data for outcomes analysis. -->

<!-- Data Fields | Description -->
<!-- ------------| -------------- -->

## Data Samples
See what a valid participants file could look like from the [templates](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/templates/participants.csv).
