# ⚡ Smart Energy Optimization Project  

## 📌 Overview  
This project focuses on **predictively minimizing energy consumption** in companies by:  
- Forecasting hourly energy demand.  
- Disaggregating usage into categories (HVAC, Lighting, Machines, IT).  
- Optimizing loads using **time-of-use tariffs**.  
- Demonstrating **cost savings & CO₂ emission reductions** through smart scheduling.  

The work is divided into **weekly milestones**.  

---

## 🚀 Week 1 – Baseline Setup  
- Generated **synthetic dataset** of company energy consumption.  
- Features included:  
  - Daily usage (kWh)  
  - Peak/off-peak usage split  
  - Smart appliance ownership  
  - Solar panel adoption  
  - EV ownership  
  - Bill amount + high bill classification  
- Ran exploratory data analysis (EDA).  
- Built **baseline ML models** for load forecasting & high bill classification.  

Notebook: [`FED_BEO.ipynb`](FED_BEO.ipynb)  

---

## 🔋 Week 2 – Load Disaggregation & Optimization  
- Extended dataset with **4 categories**:  
  - HVAC  
  - Lighting  
  - Machines  
  - IT  
- Added **Time-of-Use Tariffs**:  
  - Peak (₹10/kWh, 9AM–6PM)  
  - Mid-Peak (₹7/kWh, 7PM–10PM)  
  - Off-Peak (₹4/kWh, rest of the hours)  
- Applied **Prophet forecasting** for each load category.  
- Designed **Load Shifting Optimization** using PuLP:  
  - 50% of Machines_kWh shiftable.  
  - Shifted to off-peak hours for reduced cost.  
- Calculated:  
  - Baseline vs Optimized Cost  
  - Baseline vs Optimized CO₂ emissions  
- **Visualizations**:  
  - Baseline vs Optimized Load (first 2 days).  
  - Cost comparison bar chart.  

Notebook: [`Week2_SmartEnergy_Optimization.ipynb`](Week2_SmartEnergy_Optimization.ipynb)  

### ✅ Results (Sample Outputs)  
- 💰 **Cost Savings**: ~15–25%  
- 🌱 **CO₂ Reduction**: proportional to load shifted off-peak  

---

## 📌 Week 3: Final Submission
- Completed full Smart Energy Optimization project.  
- Finalized models for demand prediction, load optimization, and cost analysis.  
- Generated visualizations for baseline vs optimized load.  
- Submitted complete notebook: [`fED-beo.ipynb`](Week3_FinalSubmission/Fed-BEO.ipynb)


## ⚙️ Setup & Installation  

```bash
# Clone repo
git clone https://github.com/<your-username>/smart-energy-optimization.git
cd smart-energy-optimization

# Install dependencies
pip install -r requirements.txt

# Run Week 2 notebook (Colab / Jupyter)
jupyter notebook Week2_SmartEnergy_Optimization.ipynb
