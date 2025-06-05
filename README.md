# License Plate Office Simulation

This project models and compares two customer handling systems in an automotive license plate office using **Arena Simulation Software**. The aim is to analyze customer flow and identify which configuration offers better performance in terms of average and maximum time spent in the system.

## 🧪 Simulation Overview

### Simulation 1:  
- **Setup:** 3 independent arrival streams (EXPO(10 mins))  
- **Stage 1:** 3 dedicated clerks with separate queues (UNIF(8, 10) mins service time)  
- **Stage 2:** Shared clerk for all (UNIF(2.65, 3.33) mins service time)  
- **Queue Type:** Separated by customer type at first stage
![image](https://github.com/user-attachments/assets/059584d7-a758-496d-a6f1-162f81bdc5e4)

### Simulation 2:  
- **Setup:** Combined single queue  
- **Stage 1:** 3 flexible clerks serving all customers  
- **Stage 2:** Same shared clerk as Simulation 1  
- **Queue Type:** Single, shared queue for all customers
![image](https://github.com/user-attachments/assets/ad471b30-b03f-47d0-9b90-9dc10f3cf979)

Both simulations are run for a **single replication of 5,000 minutes** and the max arrival is kept at **80** per entity for simulations to avoid entity overflow.

## 📊 Objective

To compare the **average**, **minimum** and **maximum** time in the system for all customer types and evaluate which system performs better under similar arrival and service conditions.

## 🧰 Requirements

- [Arena Simulation Software](https://www.rockwellautomation.com/en-us/products/software/arena-simulation.html)

## 🚀 How to Run

1. Open the `.doe` file using Arena.
2. Click "Run" to simulate the 5,000-minute scenario.
3. Check the generated `.pdf` report for performance statistics.
4. Open `Analysis Report.docx` for conclusions and comparison between the two systems.

## 📎 Notes

- Results are based on a single replication; multiple replications can be used for more statistically accurate analysis.
- Text boxes in Arena models contain key statistics like average and maximum time in system.
