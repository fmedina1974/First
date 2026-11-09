# Data dictionary

## police_incidents.csv
- incident_id: synthetic police incident identifier
- incident_date: date incident was recorded
- region: reporting region
- offence_group: broad offence category
- outcome: current record status
- person_age: age associated with the record for practice purposes
- repeat_flag: Y/N indicator
- source_system: fictional source-system identifier

## court_matters.csv
- matter_id: synthetic court matter identifier
- incident_id: police incident identifier where linkage is available
- lodgement_date: date matter was lodged
- finalisation_date: date matter was finalised; blank means open
- court_level: Magistrates, District or Supreme
- outcome: matter outcome or Open
- region: reporting region

## corrections_admissions.csv
- admission_id: synthetic corrections admission identifier
- admission_date: admission date
- region: reporting region
- custody_type: Remand or Sentenced
- expected_release_date: synthetic expected release date

## population_monthly.csv
- month: first day of month
- region: reporting region
- estimated_population: synthetic monthly population denominator
