# Practical Network Design for Micro Edge Data Centers: An Italian Case

**Academic Research Project | KAIST (Korea Advanced Institute of Science and Technology)**

This repository contains the final report and analysis for a project on interconnection network design, focused on resource-constrained edge computing environments.

📄 **[Read the Full Report (PDF)](./Interconnection_Networks_Project_Luca_Pedercini.pdf)**

---

## 📌 Project Overview
The growing demand for low-latency applications has accelerated the deployment of edge data centers. [cite_start]However, these facilities face stringent limitations in **rack space, power availability, and budget**[cite: 171, 172].

This project investigates the trade-offs in **Clos-based network topologies** (Leaf-Spine) for edge-scale deployments. [cite_start]A specific focus is given to the **Italian context**, where regulatory and infrastructural challenges (e.g., power grid density) complicate distributed infrastructure deployment[cite: 173, 175].

## 🎯 Key Objectives
* [cite_start]**Design Space Exploration:** Analyzed five topology variants, including Full Bisection and Oversubscribed configurations (2:1, 4:3, 4:1)[cite: 174, 279].
* **Constraint Modeling:** Evaluated topologies under realistic "Micro Edge" constraints:
    * [cite_start]**Rack Space:** Max 42U[cite: 174].
    * [cite_start]**Power Budget:** Max 5kW[cite: 174].
    * [cite_start]**Cost Efficiency:** Balancing CAPEX with Bisection Bandwidth[cite: 254].
* **Optimization:** Identified the most efficient configurations to maximize performance per Euro spent.

## 🛠 Methodology & Tools
[cite_start]The analysis uses a **parametric modeling approach** rather than packet-level simulation to allow for rapid evaluation of infrastructure costs and theoretical performance[cite: 258].

* **Technologies:** Python (Pandas, Matplotlib), Google Colab Notebooks.
* [cite_start]**Architectures:** 2-Tier Clos Networks (Fat-Tree), Commodity Switches (24/48 ports)[cite: 264].
* [cite_start]**Metrics:** Total Cost (€), Power Consumption (W), Rack Units (U), Bisection Bandwidth (Gbps)[cite: 308].

## 📊 Key Findings
* [cite_start]**Oversubscription is critical:** A **2:1 oversubscription ratio** proved to be the best overall balance between cost, bandwidth, and scalability for general edge workloads[cite: 525].
* [cite_start]**Intermediate solutions:** The **4:3 ratio** emerged as a strong alternative for scenarios requiring slightly higher performance without the extreme cost of full bisection[cite: 526].
* [cite_start]**Feasibility:** Full Bisection topologies often exceed power and budget limits for micro-edge deployments, making optimized oversubscription necessary for the Italian edge scenario[cite: 519, 536].

---

## 📂 Repository Structure
