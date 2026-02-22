# Healthcare-Revenue-Cycle-Management

Technology - Azure Data Engineering Stack

Domain - Healthcare Revenue Cycle Management (RCM)

# Note : This Project is InProgress

## 📌 Roadmap

### Phase 1 – Ingestion Layer
- [x] EMR ingestion (Full + Incremental)
- [x] Metadata-driven pipeline
- [x] Claims ingestion
- [x] API integration (NPI, ICD)

### Phase 2 – Silver Layer
- [ ] Data cleaning & CDM
- [ ] SCD2 implementation

### Phase 3 – Gold Layer
- [ ] Fact & Dimension modeling
- [ ] KPI tables (AR Days, Denial Rate)

### Phase 4 – Production Readiness
- [ ] Key Vault integration
- [ ] Parallel ADF execution
- [ ] Unity Catalog
- [ ] CI/CD pipeline

Technology - Azure Data Engineering Stack

Domain - Healthcare Revenue Cycle Management (RCM)

## ADLS Gen2 Folder Structure
EMR Data - Electronic Medical Records (Azure SQL DB)
	- Patients
	- Providers
	- Department
	- Transactions
	- Encounter




Hospital a 
Hospital b 


Claims Data - Insurance company (Flat files)
folder in Datalake - Landing (monthly once)


NPI Data - National Provider Identifier (Public API)

ICD Data - ICD codes are a standardized system used by health care providers map diagnosis code and description. (API)


EMR (Database)

Claims (Flat files)

API (NPI / ICD)

Solution Architecture

Medallion Architecture

landing 	->  bronze 			-> 		silver 			->   gold

flat file   -> parquet files	->		Delta Tables	-> 	 Delta tables
