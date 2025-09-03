# TravelTide Customer Segmentation Project

## What this is
An end-to-end project that cleans **TravelTide** user activity data, engineers behavioral and value features, runs **K-Means clustering** to create customer segments, and visualizes results in a **Tableau dashboard** tied to concrete reward strategies.

## Project Link
🔗 [GitHub Repository](https://github.com/Chaitali-Arankalle/Travel-Tide-Project)

---

## Core Deliverables
- ✅ Cleaned features and segment assignments (CSV) in `data/processed`
- ✅ Packaged Tableau workbook and public link in `reports`
- ✅ Presentation deck(s) in `output`

---

## Project Contents

### Folders
- **data/raw** → Input CSVs (`users`, `sessions`, `flights`, `hotels`)
- **data/processed** → Engineered features and final segments  
  - `user_features.csv`  
  - `user_features_with_segments.csv` (features + cluster + segment name)  
  - `user_segments.csv` (user → cluster/segment lookup)  
- **scripts** → Pipeline scripts for cleaning, feature engineering, and clustering  
- **notebooks** → Exploratory and reproducible runs  
- **reports** → Tableau packaged workbook (`.twbx`) and dashboard link  
- **output** → Final slides and PDFs  

---

## Key Files to Open First
1. 📊 `reports/Travel-Tide-Segment-Analysis.twbx` → Tableau workbook  
2. 🎤 `output/TravelTide Customer Retention Case Study.pptx` → Presentation deck  
3. 📂 `data/processed/user_features_with_segments.csv` → Data behind the dashboard 
