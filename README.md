🏭 Automated Warehouse Optimization

> 📦 A logic-based simulation and planning system for automated warehouse operations using **Answer Set Programming (ASP)**.

---

## 🧠 Overview

This project models and simulates an **automated warehouse environment** using **ASP (Answer Set Programming)**. It supports parsing warehouse layouts, executing automated tasks like storage/retrieval, and planning agent movements efficiently.

---

## 📂 Project Structure

```
Automated-Warehouse/
├── convert_input.asp        # Converts raw layout/data into ASP format
├── demo.asp                 # Runs a demo simulation/logic
├── description.pdf          # 📄 Project report and logic description
├── parsing.asp              # Main ASP logic for parsing instances
├── script.py                # Python script to execute and visualize scenarios
├── simpleInstances/
│   ├── inst1.asp - inst5.asp # Sample problem instances
└── README.md                # Documentation
```

---

## ⚙️ Core Features

| 🔧 Module           | 💡 Function                                              |
| ------------------- | -------------------------------------------------------- |
| `convert_input.asp` | Translates input into ASP-readable facts                 |
| `parsing.asp`       | Encodes warehouse layout and operations logic            |
| `demo.asp`          | Runs planning logic on sample instances                  |
| `script.py`         | Automates running ASP solver on instances                |
| `simpleInstances/`  | Includes 5 sample warehouse layouts and tasks            |
| `description.pdf`   | Documentation detailing logic, planning, and methodology |

---

## 🚀 How to Run

### 🧰 Requirements

* Python 3.x
* [Clingo](https://potassco.org/clingo/) (ASP solver)

### 🏗️ Setup Clingo

Install via pip:

```bash
pip install clingo
```

Or via conda:

```bash
conda install -c potassco clingo
```

### ▶️ Run Demo (Example)

```bash
python script.py simpleInstances/inst1.asp
```

This will:

1. Parse the selected instance
2. Feed it into the ASP logic
3. Display or log the automated plan

---

## 📸 Example Use Case

Imagine a warehouse grid where:

* 📦 Items need to be stored or retrieved
* 🚚 Agents (robots) must navigate efficiently
* 🧠 The ASP engine computes an **optimal plan** for task completion

---

## 📘 Documentation

Refer to [`description.pdf`](Automated-Warehouse/description.pdf) for:

* Problem definition
* Formal logic rules
* Visualization & planning approach
* Optimization goals and constraints

---

## 📦 Sample Instances

| Instance                  | Description                                                                             |
| ------------------------- | --------------------------------------------------------------------------------------- |
| `inst1.asp` - `inst5.asp` | Represent unique warehouse layouts and item configurations to test against logic engine |
