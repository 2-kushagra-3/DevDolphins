# PySpark Data Engineer - DevDolphins Assignment

## 🧩 Overview

This project addresses the offline assignment for the **PySpark Data Engineer** role at **DevDolphins**.  
The objective is to simulate a real-time transaction ingestion and pattern detection system using:

- **PySpark** (targeting deployment on Azure Databricks)
- **Azure Blob Storage** for intermediate chunk and result storage
- **PostgreSQL** for maintaining state
- **Google Drive** as the source of the initial dataset

---

## 🚧 Note on Current GitHub State

This repository currently **only contains the offline test logic** written in **Python with pandas**, to validate and simulate the end-to-end design and pattern detection.

> The PySpark-based implementation (including full Databricks and Azure integration) **is already is done, will push the code soon** and will be pushed here shortly.

## ✅ Current Progress

As of now, the following components have been successfully developed and verified:

### 🔗 Google Drive Integration
- Authenticated using a GCP service account
- Programmatically reads the `transactions.csv` file in chunks of 10,000 rows
- Works offline as part of **Mechanism X** (the ingestion system)

### 💾 Azure Blob Storage
- Storage Account set up
- Transaction chunks are simulated locally and staged for blob upload
- Will serve as input/output location for Mechanism Y (the real-time processor)

### 🧠 PostgreSQL (Simulated)
- Intended for use as a state store for pattern detection logic
- Currently being simulated using in-memory pandas DataFrames during offline testing
- PostgreSQL Flexible Server already provisioned for future deployment

### 🔍 Pattern Detection Logic
- Detection logic for **PatId1**, **PatId2**, and **PatId3** fully implemented offline
- Modular, testable logic verified using pandas DataFrames
- State-tracking architecture implemented to support incremental processing

### ⚙️ Project Structure and Infrastructure
- Azure Databricks workspace and cluster set up
- Sample templates for Databricks config and storage provisioning are available under `templates/`
- Screenshots and architectural reference material stored under `images/`

---



---

## 🔜 Next Steps

- [ ] Finalize PySpark conversion of tested logic for Databricks deployment
- [ ] Integrate PostgreSQL as a live state store in Databricks workflows
- [ ] Write final detection outputs in batches of 50 to Azure Blob Storage
- [ ] Prepare video walkthroughs: live demo, architecture explanation, and sample outputs
- [ ] Package final submission with a downloadable zip of all output files

---

## 🧑‍💻 Author

**Kushagra Verma**  
📧 Email: kushagraid@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/2kushagraverma3/)

---

*More technical documentation, examples, and demo materials will be added as the project reaches completion.*
