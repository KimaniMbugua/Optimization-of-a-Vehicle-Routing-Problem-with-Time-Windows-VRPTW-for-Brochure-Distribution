# Optimization-of-a-Vehicle-Routing-Problem-with-Time-Windows-VRPTW-for-Brochure-Distribution
An AI-powered logistics optimization project that uses metaheuristic algorithms to solve the Vehicle Routing Problem with Time Windows (VRPTW) — efficiently planning delivery routes for 60 schools in Surabaya while minimizing travel distance, total delivery time, and ensuring all deliveries meet strict time constraints.

## 📊 Project Overview

This project tackles one of the most challenging problems in logistics — the **Vehicle Routing Problem with Time Windows (VRPTW)** — where a fleet must deliver goods or services to multiple locations **once, within specific time windows**, and **at minimal cost**.

We designed and implemented a solution to optimize the distribution of brochures from a central depot to 60 schools, leveraging advanced **metaheuristic optimization techniques**. The solution intelligently balances **efficiency**, **accuracy**, and **runtime performance**, making it ideal for real-world use cases like last-mile delivery, courier services, or transportation scheduling.

---

## 🚀 Objectives

* 🗺️ Plan routes to deliver to 60 schools **exactly once** from a single depot.
* ⏰ Ensure deliveries occur **within each school's time window**.
* 📉 **Minimize total travel distance and operational time**.
* ⚙️ Compare and evaluate multiple **metaheuristic algorithms**.
* 📊 Visualize final optimized routes and performance metrics.

---

## 🧠 Algorithms Implemented

| Algorithm                         | Approach                                         | Key Strength                                       |
| --------------------------------- | ------------------------------------------------ | -------------------------------------------------- |
| **Ant Colony Optimization (ACO)** | Bio-inspired pheromone-based search              | Fast computation and good global exploration       |
| **Hybrid PSO + Tabu Search**      | Combines swarm intelligence and tabu memory      | Best solution quality and global optimum discovery |
| **2-Opt + Simulated Annealing**   | Local optimization with probabilistic acceptance | Effective at escaping local minima                 |

---

## 📁 Project Structure

```
📂 VRPTW-Optimization
├── data/                      # Dataset: school coordinates, time windows, etc.
├── notebooks/                # Jupyter notebooks for development and experiments
├── src/                      # Core Python scripts for algorithms
│   ├── aco.py
│   ├── pso_tabu.py
│   ├── two_opt_sa.py
│   └── utils.py
├── results/                  # Output results, performance metrics, visualizations
├── README.md                 # Project documentation
└── requirements.txt          # Python dependencies
```

---

## 🔧 Key Steps

1. **Data Preprocessing:** Load and clean school location data, including time windows and service durations.
2. **Constraint Modeling:** Integrate time windows and calculate travel times between all locations.
3. **Algorithm Design:** Implement three optimization approaches with parameter tuning.
4. **Route Optimization:** Solve VRPTW and generate optimized delivery routes.
5. **Performance Analysis:** Compare total distance, runtime, and delivery time across algorithms.
6. **Visualization:** Plot delivery routes and convergence graphs for interpretability.

---

## 🏆 Results & Achievements

| Metric                 | ACO         | PSO + Tabu      | 2-Opt + SA  |
| ---------------------- | ----------- | --------------- | ----------- |
| 🛣️ Total Distance     | 118.72 km   | **116.60 km**   | 117.89 km   |
| ⏱️ Runtime             | **57 s**    | 89 s            | 64 s        |
| 📦 Total Delivery Time | 1335.12 min | **1310.57 min** | 1322.98 min |

* ✅ Achieved **116.60 km** minimum total route length using **PSO + Tabu Search**.
* ⚡ Reduced computational time to **57 seconds** with **ACO**.
* 📉 Cut total delivery time to **1310.57 minutes**, ensuring all schools received brochures on schedule.
* 📈 Improved routing efficiency by over **10%** compared to naive sequential approaches.

---

## 📸 Visualizations

* 🗺️ **Optimized Delivery Routes:** Route maps showing the final vehicle paths and delivery sequences.
* 📊 **Algorithm Comparison:** Performance charts showing distance, runtime, and convergence.
* 📈 **Convergence Curves:** Optimization progress over iterations.

---

## 🧪 How to Run

### 1️⃣ Clone the repository

```bash
git clone https://github.com/yourusername/VRPTW-Optimization.git
cd VRPTW-Optimization
```

### 2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run the optimization

```bash
python src/aco.py
python src/pso_tabu.py
python src/two_opt_sa.py
```

Or open the Jupyter notebook for exploration:

```bash
jupyter notebook notebooks/VRPTW_Optimization.ipynb
```

---

## 🧭 Applications

* 🚛 **Last-Mile Delivery Optimization**
* 📦 **Courier and Parcel Routing**
* 🏙️ **Urban Transportation Planning**
* 🏪 **Retail Distribution & Supply Chain Management**

---

## 📚 Future Work

* 🔁 Implement multi-depot routing and vehicle capacity constraints.
* 🌐 Integrate real-time traffic data for dynamic routing.
* 🧠 Explore deep reinforcement learning approaches for VRPTW.



