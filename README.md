# Transjakarta Route & Stop Optimization  
### Using Exploratory Data Analysis (EDA) and Diagnostic Analysis

This project analyzes operational efficiency across Transjakarta bus routes and stops using Exploratory Data Analysis (EDA) and Diagnostic Analysis.  
The goal is to identify underutilized and overcrowded routes, imbalanced travel directions, and high-impact OD (Origin–Destination) pairs, then deliver actionable recommendations to optimize fleet distribution and improve overall operational performance.



## 1. Project Summary  

Transjakarta operates one of the largest BRT (Bus Rapid Transit) networks in Southeast Asia. Passenger demand varies significantly by hour, corridor, direction, and day type.  
Without proper optimization, this leads to:

- Overcrowded buses during peak hours  
- Idle buses on low-demand routes  
- Inefficient fleet allocation  
- Higher operational cost  
- Lower occupancy and lost revenue opportunity  

This project provides **data-driven insights** to improve:

- Route efficiency  
- Stop-level effectiveness  
- Directional balance  
- Fleet distribution  
- Operational cost efficiency  
- Passenger experience  

**Dataset Source:** Internal project dataset provided for Purwadhika Data Science Bootcamp (Capstone Module 2).



## 2. Repository Structure

```
transjakarta-route-and-stop-optimization/
├── transjakarta_route_stop_analysis.ipynb   # full EDA & diagnostic analysis
└── README.md                                # project documentation
```


## 3. Tools & Technologies

| Category        | Tools                                 |
|----------------|----------------------------------------|
| Programming    | Python (Pandas, NumPy)                 |
| Notebook       | Jupyter Notebook                       |
| Visualization  | Tableau                                |
| Data Format    | CSV, Excel                             |
| Version Ctrl   | Git & GitHub                           |



## 4. Analysis Components

### **4.1 Hourly Demand Analysis**
- Two strong peaks: **06:00** and **17:00**  
- Mid-day demand drops to **<5% of peak level** → major opportunity to optimize off-peak frequency

### **4.2 Weekday vs Weekend**
- Weekend demand = **20–30% of weekday volume**  
- Without frequency adjustment, many buses will run empty

### **4.3 Stop Demand Segmentation**
Stops are categorized into:
- **High demand** (Top 25%)  
- **Medium demand** (Middle 50%)  
- **Low demand** (Bottom 25%)  

> Many stops contribute **<1%** of total demand → operational inefficiency.

### **4.4 Corridor Performance**
- Several corridors are over-utilized  
- Key corridors generate **20–23×** higher trips than low-performing ones  
- Large imbalance signals fleet misallocation

### **4.5 Direction Gap Analysis**
- Maximum imbalance: **10 trips difference**  
- One direction heavily dominates → even fleet distribution is inefficient

### **4.6 OD Matrix Analysis**
- <5% of OD pairs contribute the majority of total trips  
- >80% OD pairs have very low utilization → high redundancy



## 5. Key Insights

- Demand is **highly uneven** by hour, corridor, direction, and day type  
- Overcrowded corridors require reinforcement  
- Many stops have minimal usage → potential for reallocation  
- Weekend operations need restructuring  
- Premium OD routes dominate traffic  
- Directional imbalance indicates poor alignment between fleet and passenger flow  



## 6. Recommendations

### **1. Reinforce High-Demand Corridors**
- Add buses to heavy corridors  
- Reduce waiting time during peak hours  

### **2. Apply Dynamic Headway**
- Tighten headway at peak (06:00 & 17:00)  
- Extend headway at off-peak (10:00–15:00) to cut empty trips  

### **3. Optimize Weekend Operations**
- Demand only 20–30% → reduce frequency to avoid idle buses  

### **4. Reallocate Resources from Underutilized Corridors**
- Move idle buses to high-demand routes  
- Maintain minimum operational threshold only where required  

### **5. Balance Directional Flow**
- Increase supply on dominant direction (gap up to 10 trips)  
- Reduce opposing direction to minimize empty returns  

### **6. Prioritize Premium OD Routes**
- Focus planning on <5% OD pairs contributing majority of traffic  
- Maintain high reliability for core commuter flows  



## 7. Author  

**Hanna Muthie**  
Purwadhika Data Science Bootcamp  
GitHub: https://github.com/hannms  



## 8. How to Run This Project

1. Download the Jupyter Notebook (`.ipynb`).  
2. Open in Jupyter Notebook or VS Code.  
3. Run all cells to reproduce the analysis and results.  




Thank you for viewing this project!  
This repository is part of **Purwadhika Data Science Bootcamp – Capstone Module 2**.
