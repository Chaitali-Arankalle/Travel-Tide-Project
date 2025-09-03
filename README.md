# TravelTide Segmentation Project

## 📌 Overview
This project focuses on building **customer segments** for TravelTide to improve retention and loyalty through targeted rewards.  
The workflow is designed to be clean, structured, and easy to run in **Google Colab** or locally.

We transform raw travel data (`users`, `sessions`, `flights`, `hotels`) into meaningful features, apply clustering, and export results for business analysis in **Tableau**.  
Final outputs are provided in the form of **data files, a written document, and a presentation**.

---

## 📂 Project Structure
- **data/raw/** → Contains input data (users, sessions, flights, hotels).  
- **data/processed/** → Contains cleaned data and final user-level features with cluster labels.  
- **output/models/** → Placeholder for saved machine learning models.  
- **reports/** → Cluster profiles, evaluation metrics, and written project documentation.  
- **presentation/** → Slide deck summarizing business problem, approach, segmentation, and outcomes.  
- **scripts/** → Contains the main segmentation script.  
- **README.md** → Project documentation.  

---

## 🔄 Workflow

### 1. Setup & Project Paths
- Mounted Google Drive in Colab.  
- Created folders for raw data, processed data, models, reports, and scripts.  

### 2. Data Connection
- Input can come from **CSV files** or directly from the **Postgres database**.  
- The four core tables are: `users`, `sessions`, `flights`, `hotels`.  

### 3. Data Cleaning
- Converted timestamps, fixed missing hotel nights, standardized numeric fields.  
- Derived new features (e.g., session duration).  
- Removed duplicates.  

### 4. Exploratory Data Analysis (EDA)
- Sanity checks with histograms and distributions.  

### 5. Feature Engineering
- Built user-level metrics across sessions, flights, and hotels.  
- Created **RFM-style features** (Recency, Frequency, Monetary).  
- Added behavioral metrics (cancellation rate, booking rate, engagement).  
- Applied cohort filtering and handled outliers.  

### 6. Segmentation (K-Means)
- Standardized features.  
- Evaluated multiple cluster sizes (k = 3–6) using **silhouette score**.  
- Selected best `k` and assigned clusters to users.  
- Built cluster profiles for interpretation.  

---

## 📊 Outputs

### Data files (CSV)
- `customer_segments.csv` → complete dataset with clusters.  
- `user_features.csv` → simplified, Tableau-ready.  

### Document (PDF/Markdown)
- Step-by-step explanation of the workflow, decisions, and results.  

### Presentation (Slides)
- Business problem → Solution approach → Feature engineering → Segmentation results → Recommendations.  

---

## 🏢 Business Integration
- Tableau dashboards built on `user_features.csv` help visualize segment sizes, KPIs, and retention trends.  
- The **document** serves as a technical summary for analysts.  
- The **presentation** communicates the business story and recommendations to stakeholders.  

---

## ✅ Key Takeaways
- Built a reproducible pipeline for TravelTide segmentation.  
- Delivered **data + document + presentation** for both technical and business audiences.  
- Supports strategic design of customer rewards and retention programs.  
