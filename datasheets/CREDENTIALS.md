# Data Sheet for Credentials
The description of required and recommended fields for credentials data follows. Credentials data files for upload may include any additional fields not listed here.

## Required Fields
The outlined fields are required to derive the required set of provider outcomes. Field header names used relate closely with those used in the [Credentials Registry](http://credreg.net/) but files uploaded need not use the same field header names.

Data Fields | Description
------------| --------------
**program_provider** | Name of provider offering a training program. This may be a college(2-year or 4-year), vocational institute or organization offering programs
**program_code** | Numeric code uniquely identifying the category in which program falls, e.g Classification of Instructional Programs(CIP) code for the program
**credential_name** | Full name of the credential offered for program
**credential_description** | Full description of the credential as offered by provider for the associated program
**credential_type** | Type of credential obtained e.g `Associate Degree`, `Bachelors Degree`, `Apprenticeship Certificate`. These credential types match up the [Credentials Registry Mapping of `Credential Type`](http://credreg.net/ctdl/mapping/registry)
**credential_status_type** | Status of credential as outlined by [Credentials Status Registry Vocabulary](http://credreg.net/registry/assistant#vocab_CredentialStatus). Valid status types are `Active`, `Deprecated`, `Probationary`, `Superceded`
**audience** | The intended audience for the program for which this credential is granted e.g `Resident`, `FormerMilitary`, `PublicEmployee`. See full list of audiences in [Audience Credentials Registry Vocabulary](http://credreg.net/registry/assistant#vocab_Audience)
**audience_level** | The current credential/training level of the above audience e.g `AdvancedLevel`, `AssociatesDegreeLevel`, `BachelorsDegreeLevel`, `SecondaryLevel`, `PostSecondaryLevel`. See full list of audience levels in [Audience Level Credentials Registry Vocabulary](http://credreg.net/registry/assistant#vocab_AudienceLevel)
**language** | Primary language of the credential

## Recommended Fields
The following fields are not required but they are recommended to provide more credentials data captured by the [Credentials Registry](http://credreg.net/).

Data Fields | Description
------------| --------------
**ctid** | If available, [Globally unique Credential Transparency Identifier (CTID)](http://credreg.net/ctdl/terms/ctid#ctid) by which the provider of a credential recognizes the (credential) entity in transactions with the external environment (e.g., in verifiable claims involving a credential)
**webpage** | URL for the webpage that describes the credential. If this is not included with credentials data, the   `program_website` in the [Programs Required Fields](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/datasheets/PROGRAMS.md#required-fields) for the associated program is assumed


## Data Samples
See what a valid credentials file could look like from the [templates](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/templates/credentials.csv).
