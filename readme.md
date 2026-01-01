## 📚 Data Source

This hospital database is sourced from **Maven Analytics**.

- Dataset: Hospital Patient Records  
- Provider: [Maven Analytics](https://mavenanalytics.io/data-playground/hospital-patient-records)
- Tool: ![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-blue).

The dataset is used for learning and educational purposes.

### DATASET
- Total Patients (974)
```sql
SELECT COUNT(*) FROM patients;
```
- Total Encounters:27891
```sql
SELECT COUNT(*) FROM encounters;
```
- Data Range: 2021-2022

## :card_file_box: Database Tables
- patients
- encounters
- procedures
- oganizations
- payers


### Basic Table Inspection Queries
```sql
SELECT * FROM patients;
SELECT * FROM encounters;
SELECT * FROM procedures;
SELECT * FROM organizations;
SELECT * FROM payers;
```

### Table Structure Example (patients)
```sql
SELECT column_name, data_type
FROM information_schema.columns
WHERE table_name = 'patients';
