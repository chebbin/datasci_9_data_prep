# datasci_9_data_prep
data prep for ML 

## Dataset #1
https://data.chhs.ca.gov/dataset/11c64371-5d52-4d08-831a-e553528e661f/resource/f1a5afce-5d94-4126-9b0c-bffefc388337/download/2019-2020-homeless-ip-and-ed-by-facility.csv

2019-2020 Homeless Hospital Encounters: Age, Race, Sex, Expected Payer By Facility
This dataset contains counts of inpatient hospitalizations and emergency department visits for persons experiencing homelessness and non-homeless patients; stratified by age group, race/ethnicity, sex, and expected payer.  Other Payer includes Workers’ Compensation, Other Government, Title V, Disability, VA Plan, Other Payer, invalid, and missing.

### Intended ML task
This preparation will be for a classification task to predict homelessness

### Data Cleaning and Transformation Plan
1. First load in the dataset
2. Drop missing values
3. Edit the dataset to include only columns of interest
4. Edit the Demographic column to only include rows that describe the payer
5. Drop the Demographic column as it now only has one value
6. Encode categorical values for columns that are not numerical

### The variables
Independent variables: Urban_Rural, Teaching, DemographicValue,	Encounters,	TotalEncounters, Percent
Dependent variable: HomelessIndicator

### Data Splitting
Performed using the above variables for X as the independent variables and y as the dependent variable

## Dataset #2
https://healthdata.gov/resource/a8v3-a3m3.csv?$query=SELECT%20district_nces_id%2C%20district_name%2C%20week%2C%20learning_modality%2C%20operational_schools%2C%20student_count%2C%20city%2C%20state%2C%20zip_code%20ORDER%20BY%20week%20ASC

### Intended ML task
This preparation will be for a classification task to predict the learning modality which can be in-person, remote, or hybrid

### Data Cleaning and Transformation Plan
1. First load in the dataset
2. Drop missing values
3. Edit the dataset to include only columns of interest
4. Check for variable types, and then change the zip code column from an integer to a string
5. Encode categorical values for columns that are not numerical

### The variables
Independent variables: week, operational_schools,	student_count, zip_code
Dependent variable: learning_modality

### Data Splitting
Performed using the above variables for X as the independent variables and y as the dependent variable








