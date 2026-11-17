# Startup Expansion Analysis (`Startup-Expansion-Analysis-`) — K-Means Market Segmentation & Power BI

A hybrid **Python Machine Learning & Power BI** analytics project combining unsupervised **K-Means clustering** (`Untitled-1.ipynb`) with executive BI dashboards (`nm.pbix`) to evaluate startup expansion opportunities across regions and spend profiles.

---

## 1. Executive Summary & Purpose
`Startup-Expansion-Analysis-` guides data-backed market expansion decisions by cleaning raw expansion metrics (`startup-expansion.xlsx`), segmenting markets via `KMeans` clustering (`modified.csv`), and visualizing ROI and expansion performance in Power BI (`nm.pbix`).

## 2. Pipeline Architecture & Layers
```mermaid
flowchart LR
    Raw["startup-expansion.xlsx"] --> Prep["LabelEncoder & StandardScaler"]
    Prep --> Cluster["KMeans Clustering (Untitled-1.ipynb)"]
    Cluster --> Out["modified.csv"]
    Out --> BI["Power BI Executive Report (nm.pbix)"]
```

| Layer | Tools & Artifacts |
| :--- | :--- |
| **Data Ingestion & Prep** | `pandas`, `numpy`, `LabelEncoder`, `StandardScaler` (`startup-expansion.xlsx`) |
| **Unsupervised ML Layer** | `sklearn.cluster.KMeans` segmentation (`Untitled-1.ipynb`) |
| **BI & Visualization Layer** | `matplotlib`, `seaborn`, and Power BI (`nm.pbix`, `modified.csv`) |

## 3. Getting Started
```bash
git clone https://github.com/islamsamyy/Startup-Expansion-Analysis-.git
cd Startup-Expansion-Analysis-
jupyter notebook Untitled-1.ipynb
```

## 4. Business Value & Growth Opportunities
- **Capital Allocation Efficiency**: Prevents over-investing in low-yield territories by grouping cities/branches into high-ROI vs. high-risk expansion clusters.
- **Franchise & SaaS Site Selection**: Extend the K-Means pipeline with demographic and competitor-density feeds to offer automated territory-scoring for retail and startup expansions.
