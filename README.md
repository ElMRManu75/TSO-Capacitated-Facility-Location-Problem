# Capacitated Facility Location Problem (CFLP)

This project addresses the classical combinatorial optimization problem known as the **Capacitated Facility Location Problem (CFLP)**, using a greedy constructive heuristic and a local search algorithm. It is implemented in Python as part of the course **Advanced Topics in Optimization** at the Universidad Autónoma de Nuevo León.

## 📌 Problem Description

The CFLP involves deciding **which facilities to open** and **how to assign customers to those facilities** in a way that:
- **Minimizes total cost** (fixed costs + assignment costs),
- Respects the **capacity constraints** of each facility,
- **Satisfies all customer demands**.

This problem has practical applications in logistics, supply chain management, telecommunications, healthcare, and more.

## 🧠 Project Approach

### 1. **Greedy Constructive Heuristic**
- Assigns customers to facilities based on a composite cost:  
  `(assignment cost + fixed cost per unit of demand)`
- Prioritizes already-open facilities before considering new ones.

### 2. **Local Search**
- Improves the initial solution using two operations:
  - **Closing open facilities** and reassigning their clients.
  - **Opening closed facilities** and reassigning clients to reduce costs.
- Uses a **best improvement** strategy.

## ⚙️ System Specifications

- **Processor:** Intel Core i7-10750H @ 2.60GHz  
- **RAM:** 16 GB  
- **Operating System:** Windows 11 Home 64-bit  
- **Programming Language:** Python 3.11  
- **Libraries Used:**  
  - `numpy`  

## 📊 Instances Used

We used 15+ instances from the academic repository:

🔗 [Guastaroba & Speranza SSCFLP Instances](https://or-brescia.unibs.it/instances/instances_sscflp)

Each file includes:
- Number of facilities and customers,
- Facility capacities, customer demands,
- Fixed costs and assignment costs.

## 📈 Results

- On average, local search improves the greedy solution by approximately **2.4%**.
- Execution time increases with instance size.
- Compared to optimal values, some improvements exceed **600%**.

## 📬 Contact

Project Team:
- Abraham Bernacho Mares
- Angela Daniela Vazquez Gutierrez
- Cesar Alejandro Flores Perez
- Santiago Isaac Flores González
- Luis Alberto Rodríguez Rojas
- Juan Manuel Ramos Obregon

Professor: **Dr. María Angélica Salazar Aguilar**  
Course: *Advanced Topics in Optimization - Jan-Jun 2025*  
Faculty of Mechanical and Electrical Engineering - UANL
