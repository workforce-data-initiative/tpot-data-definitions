# Data Sheet for Credentials
The description of required and recommended fields for credentials data follows. Credentials data files for upload may include any additional fields not listed here.

## Required Fields
The outlined fields are required to derive the required set of provider outcomes. Field header names used relate closely with those used in the [Credentials Registry](http://credreg.net/) but files uploaded need not use the same field header names.

Data Fields | Description
------------| --------------
**program_code** |  Unique ID identifying the program e.g Classification of Instructional Programs(CIP)
**credential_name** | Full name of the credential offered
**credential_type** | Type of credential obtained e.g Associate Degree, Bachelors Degree, Apprenticeship Certificate
**CTID** | [Globally unique Credential Transparency Identifier (CTID)](http://credreg.net/ctdl/terms/ctid#ctid) by which the provider of a credential recognizes the (credential) entity in transactions with the external environment (e.g., in verifiable claims involving a credential).

## Recommended Fields
The following fields are not required but they are recommended to provide more credentials data captured by the [Credentials Registry](http://credreg.net/).

Data Fields | Description
------------| --------------
**program_name** | Name of program being offered by the training provider
**credential_status_type** | Status of credential as outlined by [Credentials Registry Vocabulary](http://credreg.net/registry/assistant#vocab_CredentialStatus). Valid status types are `Active`, `Deprecated`, `Probationary`, `Superceded`
**delivery_type** | This relates closely with the `program_offering_model` [recommended programs field](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/datasheets/PROGRAMS.md#recommended-fields)
**learning_method** | Types of methods used to conduct the learning opportunity e.g `Lecture`, `Seminar`, `Online`
<!-- **audience** | -->
<!-- **credential_audience_level** | -->
