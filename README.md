# Summer-Analytics-2025-x-IIT-Guhawati-Capstone-Project

# -Capstone-Project-x-IIT-Guhawati-         

# Dynamic Pricing for Urban Parking Lots

**Capstone Project – Summer Analytics 2025**  
**Author:** Himanshu Kundan Tapde  
**Date:** 07th July 2025  

---


## 🔗 Links to the Project Files

## Interactive Bokeh Visualizations (HTML version):
View the interactive Bokeh version with pricing and rerouting suggestions
https://github.com/Himanshu431-coder/Summer-Analytics-2025-x-IIT-Guhawati-Capstone-Project/blob/main/cleaned_Capstone_Project_by_Himanshu_Tapde.html


## Google colab Notebook (Code and Analysis):
View the google colab notebook (Code + Static Outputs)
https://github.com/Himanshu431-coder/Summer-Analytics-2025-x-IIT-Guhawati-Capstone-Project/blob/main/cleaned_Capstone_Project_by_Himanshu_Tapde.ipynb



## 🚀 Project Overview
Urban parking is scarce and demand‐driven. This project builds a streaming pricing engine for 14 parking lots using Pathway, pandas, and numpy.  
We implement three pricing models of increasing sophistication:
1. **Model 1: Baseline Linear**  
2. **Model 2: Demand‐Based**  
3. **Model 3: Competitive** + **Overflow Rerouting**  

Interactive Bokeh dashboards visualize real‐time prices and reroute suggestions.

---

## 🛠️ Tech Stack
- Python 3.8+  
- Pandas, NumPy  
- [Pathway](https://pathway.com/) for real‐time streaming  
- Geopy for distance calculations  
- Bokeh for interactive visualization
- Matplotlib for extra visuals  
- Google Colab (execution environment)

---

## 📁 Repository Structure
parking-dynamic-pricing/
├── README.md
├── requirements.txt
├── Capstone Project by Himanshu Tapde.ipynb
├── dataset.csv
├── prices.csv
└── docs/
  
---

## 📐 Architecture Diagram

![Screenshot (52)](https://github.com/user-attachments/assets/36827c91-407e-4519-82cb-ac9442edfa1e)


## 🔧 Project Workflow

## Data Simulation

A CSV‐based simulator emits time‐stamped lot states into a Pathway stream

## Model 1: Baseline Linear

price_{t+1} = price_t + α × (occupancy/capacity)

Serves as reference

## Model 2: Demand‐Based

Composite demand score from occupancy rate, queue length, traffic, special‐day, vehicle type

Normalized and bounded between 0.5× and 2× base price

## Model 3: Competitive

For each lot at capacity, looks at neighbors (≤1 km)

If cheaper → −5%; if more expensive → +5%

## Overflow Rerouting

When a lot is full, suggest up to 3 cheapest non-full neighbors

## Visualization

Interactive Bokeh plots:

Green: Model 2 prices

Red: Model 3 prices

Blue markers: competitive adjustments

Hover shows reroute suggestions


## 📥 Installation & Execution

Copy & paste the commands below to get started:

```bash
# 1. Clone your repository
git clone https://github.com/Himanshu431-coder/Capstone-Project-x-IIT-Guhawati-.git
cd Capstone-Project-x-IIT-Guhawati-

# 2. Install Python dependencies
pip install -r requirements.txt

Then, in Google Colab:

1.Open the notebook Capstone Project by Himanshu Tapde.ipynb (File → Open notebook → GitHub → paste your repo URL)

2.Upload your input data

3.Drag & drop dataset.csv into the Colab file browser (left panel)

4.Run all cells

5.Runtime → Run all

6.Download the result After the final cell writes /tmp/prices.csv, add & run:

```bash
from google.colab import files
files.download('/tmp/prices.csv')


## 📧 Contact
For questions, suggestions, or collaboration, feel free to reach out:

Email: himanshutapadia312@gmail.com

GitHub: https://github.com/Himanshu431-coder/

