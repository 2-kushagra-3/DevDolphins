## 🧩 Overview

The objective is to simulate and implement a near real-time transaction ingestion and pattern detection system using:

* **PySpark** (for production on **Azure Databricks**)
* **Azure Blob Storage** for intermediate chunk storage and result output
* **PostgreSQL** for maintaining incremental state
* **Google Drive** as the source for the initial raw dataset


---

## ✅ Current Progress

### 🔗 Google Drive Integration

* Authenticated using a **GCP service account**
* Reads the **transactions.csv** file in programmatically controlled chunks (10,000 rows each)
* Validated offline as **Mechanism X** (the data ingestion component)

### 💾 Azure Blob Storage

* **Storage Account** is provisioned and working
* Transaction chunks are staged locally and uploaded to Blob (simulated)
* Will serve as the **input/output store** for **Mechanism Y** (the streaming processor)

### 🧠 PostgreSQL (Simulated)

* Designed to act as a **state store** for incremental pattern detection
* Fully simulated using **in-memory pandas DataFrames** for offline testing
* **PostgreSQL Flexible Server** is provisioned for Databricks integration

### 🔍 Pattern Detection Logic

* Detection logic for **PatId1**, **PatId2**, and **PatId3** fully implemented and verified offline and on databricks
* Modular, incremental logic matches the real-time streaming design
* Offline prototype successfully reproduces state updates, detection thresholds, and output batching
* PySpark conversion now validated with **AutoLoader**, **state writes to PostgreSQL**, and batch output to Blob

### ⚙️ Project Infrastructure

* **Azure Databricks** workspace and cluster are set up
* Sample **Databricks notebooks**, configuration templates, and connection helpers included under `/templates/` (will be updated with final notebooks)

---

## 👤 Author

**Kushagra Verma**
📧 [kushagraid@gmail.com](mailto:kushagraid@gmail.com)
🔗 [LinkedIn](#) *((https://www.linkedin.com/in/2kushagraverma3/))*

---

**More technical documentation, detailed examples, and a final deployment-ready demo will be added as the project is finalized.** 🚀✨
