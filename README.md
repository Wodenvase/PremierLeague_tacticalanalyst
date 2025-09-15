
# Premier League Team Playstyle Analysis ⚽📊

This project uses **unsupervised machine learning** to analyze team performance data from the Premier League.  
The goal is to move beyond simple league standings and identify distinct tactical profiles or **"playstyles"** of the teams.  
We apply **Principal Component Analysis (PCA)** for dimensionality reduction and **K-Means Clustering** to group teams with similar statistical DNA.

---

## 🌟 Key Features

- **Automated Data Collection** → Scrapes the latest league data from FBref.  
- **Structured Workflow** → Clean, five-notebook pipeline for reproducibility.  
- **Unsupervised Learning** → Uses PCA + K-Means to uncover tactical clusters.  
- **Rich Visualizations** → Includes:  
  - 2D Tactical Map of teams  
  - Cluster "DNA" Radar Charts  
  - Heatmaps & Violin Plots for deeper insights  

---

## 📂 Project Structure

Tactical_Analyst/
│
├── data/
│   ├── raw_team_data.csv
│   ├── processed_team_data.csv
│   └── clustered_team_data.csv
│
├── 01_Data_Collection.ipynb             # Scrapes raw data from FBref
├── 02_Data_Preprocessing.ipynb          # Cleans & scales features
├── 03_Modeling_PCA_KMeans.ipynb         # PCA + K-Means clustering
├── 04_Visualization_and_Interpretation.ipynb  # Tactical map + initial analysis
├── 05_Deeper_Insights_and_Visualizations.ipynb # Radars, heatmaps, violin plots
└── README.md

---

## 🧠 Methodology

1. **Data Scraping** → Collects team-level stats (Goals, xG, xGA, etc.) from FBref.  
2. **Preprocessing** → Cleans + scales numerical features using `StandardScaler`.  
3. **Dimensionality Reduction (PCA)** → Reduces multiple features into 2 principal components, interpreted as tactical axes (e.g., *Overall Quality* vs. *Attack vs. Defense Bias*).  
4. **Clustering (K-Means)** → Groups teams into clusters, with optimal **k** chosen using the **Elbow Method**.  

---

📈 Visualizations Showcase
This scatter plot places each team on a 2D map based on their two principal components and plots them by their assigned cluster. It provides a high-level overview of the tactical landscape of the league.
(You can add a screenshot of your plot here)
![Performance Map](images/Performance_chart.png)

---

## 🚀 How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/Tactical-Analyst.git
cd Tactical-Analyst
'''
2. Create Virtual Environment (Recommended)

python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

3. Install Dependencies

Create a requirements.txt file:

pandas
scikit-learn
matplotlib
seaborn
lxml

Install with pip:

pip install -r requirements.txt

4. Run the Notebooks in Order

Open Jupyter Notebook/Lab and execute:
	1.	01_Data_Collection.ipynb
	2.	02_Data_Preprocessing.ipynb
	3.	03_Modeling_PCA_KMeans.ipynb
	4.	04_Visualization_and_Interpretation.ipynb
	5.	05_Deeper_Insights_and_Visualizations.ipynb

⸻

📊 Data Source

All statistics are sourced from FBref.
This project is intended for educational purposes only.

⸻

📜 License

Released under the MIT License.

Do you also want me to **add badges (Python version, License, Last Commit)** at the very top, like I did in the market regimes README, to give it a more open-source look?
