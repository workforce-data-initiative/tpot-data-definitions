
# Data Sheet for WIOA Participants

The description of required and recommended fields for [Workforce Innovation and Opportunity Act(WIOA)](https://www.doleta.gov/WIOA/Overview.cfm) participants data follows. These fields are based on the Participant Individual Record Layout (PIRL) 

## Required Fields

The outlined fields are required to derive a minimal set of training provider outcomes. It is highly recommended that files uploaded use similar field header names (for both these required fields and recommended fields below)

Data Fields | Description
------------| --------------
**participant_id** | Unique ID identifying a program participant throughout period of participation, e.g a Social Security Number. Participant unique identification supports operations like wage matching for outcomes derivation
**state_of_residence** | 2-letter FIPS alpha code of the state or territory of the primary domicile (location established or claimed as the permanent residence or "home") of the participant. e.g the State of Alabama would be represented as `AL`
**adult** | Is participant receiving WIOA support as an individual over the age of 18? Indicated with numeric values, `1 = Yes, Local Formula`, `2 = Yes, Statewide`, `3 = Yes, Both Local and Statewide`, `0 = No`
**dislocated_worker** | Numeric value indicating whether participant received services financially assisted under the respective WIOA section. Options are, `1 = Yes, Local Formula`, `2 = Yes, Statewide`, `3 = Yes, Both Local and Statewide`, `0 = No`
**youth** | Numeric value indicating whether participant received services financially assisted under the respective WIOA section. Options are, `1 = Yes, Local Formula`, `2 = Yes, Statewide`, `3 = Yes, Both Local and Statewide`, `0 = No`
**adult_education** | Numeric value indicating whether participant received services financially assisted under WIOA Title II. Valid options are, `1 = Yes`, `0 = No`, `9 = Unknown`
**entry_date** | Date participant commenced the program, this may differ from the enrollment date and the official date of program commencement set by the provider, in the format `YYYYMMDD`
**exit_date** | Date participant exited the program, in the format `YYYYMMDD`
**exit_type** | Nature of participant's exit from the program e.g `Graduated`, `Transferred` etc. This maps to the [`program_potential_outcome` in the Programs required fields](https://github.com/workforce-data-initiative/tpot-data-definitions/blob/master/datasheets/PROGRAMS.md#required-fields)
**exit_reason** | For individuals that exit program based on exit types related to abandonment of program, use any of these numeric values to capture why, `01 = Institutionalized`, `02 = Health/Medical`, `03 = Deceased`, `04 = Reserve Forces called to Active Duty`, `05 = Foster Care`, `06 = Ineligible`, `99 = Not a Valid SSN`, `00 = Other`. There is also an additional option, `98 = Retirement`
**employment_type_exit_q1** | Numeric value denoting type of employment individual is engaged in during the 1st quarter after they exit the program in which they were enrolled. Options are, `1 = State wage records`, `2 = WRIS wage records`, `3 = Federal Employment Records(OPM)`, `4 = Military Employment Records(DOD)`, `5 = Other Administrative Wage Records`, `6 = Supplemental through case management, participant survey, and/or verification with the employer`, `7 = Information not yet available`, `0 = Not employed`
**ita** |  Boolean: is individual receiving WIOA Title I funding via an ITA? 
**date_of_birth** | Participant date of birth in the format `YYYYMMDD`. Note that this is mandatory for Vocational Rehabilitation (RSA)
**gender** | Numeric value indicating participant gender as `1 = Male`, `2 = Female`, `9 = Participant did not self-identify`
**ethnicity** | PIRL offers 7 field options: `Hispanic/Latino`, `American Indian/Alaska Native`, `Asian`, `Black/African American`, `Native Hawaiian/Other Pacific Islander`, `White`, `More Than One Race`  . For any one of these captured for a participant, ethnicity is recorded as `1 = Yes`, `0 = No`, `9 = Participant did not self-identify`
**employment_status** | Numeric value indicating participant employment status at the time of entry into a program. Options are: `1 = Employed`, `2 = Employed, but Received Notice of Termination of Employment or Military Separation`, `3 = Not in labor force`, `0 = Not Employed`
**displaced_homemaker** | Numeric value, `1 = Yes`, `0 = No`, indicating whether or not participant has been providing unpaid services to family members in the home and was dependent on income from another family member but is no longer supported, or is experiencing reduced support due to (military) deployment of family member, or is underemployed/unemployed with difficulty obtaining/upgrading employment
**low_income** | Numeric value, `1 = Yes`, `0 = No`, indicating whether or not participant is considered low income as per federal and/or state designations. See `[PIRL]() No.702` for details
**person_with_disability** | Numeric value used to record whether participant indicated having any disability, `1 = Yes`, `0 = No`, `9 = Participant did not disclose`
**ex_offender** | Numeric value, `1 = Yes`, `0 = No`, indicating whether or not participant has been subject to the crimimal justice process through commission of an offense or faces artificial barriers to employment because of arrest or conviction record
**homeless_runaway** | Numeric value, `1 = Yes`, `0 = No`, indicating whether or not participant is a homeless individual or runaway youth at program entry.
**foster_care** | Numeric value, `1 = Yes`, `0 = No`, indicating whether or not participant in this program of study who are youth up to age 24 who have ever been in, or have aged out of the foster care system, at program entry.
**english_learner** | Numeric value, `1 = Yes`, `0 = No`, indicating whether or not participant in this program of study is an English language learner, an individual who has low levels of literacy, or who faces substantial cultural barriers at program entry.
**migrant_seasonal** | Numeric value, `1 = Yes`, `0 = No`, indicating whether or not participant in this program of study is a migrant or seasonal farmworker at program entry.
**exhausting_tanf** | Numeric value, `1 = Yes`, `0 = No`, indicating whether participant in this program of study at program entry will exhaust TANF (Part A Title IV of the Social Security Act) within 2 years.
**single_parent** | Numeric value, `1 = Yes`, `0 = No`, indicating whether participant in this program of study is a single parent or single pregnant women at program entry.
**long_term_unemployed** | Numeric value, `1 = Yes`, `0 = No`, indicating whether participant in this program of study is long-term unemployed at program entry.
