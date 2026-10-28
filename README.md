# Python Computational Logic Case Studies Repository

A comprehensive suite of 10 computational logic projects designed, implemented, and documented as part of the CSE Python Programming coursework. Each project contains a fully functional Python engine, mathematical formulation, system flowchart, test cases, and diagnostic reporting.

---

## 📄 Author & Metadata

* **Name:** P. Sai Sudha
* **Branch & Section:** CSE-1
* **Roll Number:** 261000051
* **Language:** Python 
* **Framework:** Standard Library (`dataclasses`, `math`, `re`, `typing`)

---

## 📚 Overview of the 10 Computational Logic Projects

| # | Project Name | Primary Focus / Key Features |
|---|---|---|
| **1** | **Progressive Electricity Billing System** | Tiered energy slabs, regulatory surcharges, tax/rebate calculation, consumption spike anomaly detection (>25%). |
| **2** | **Laboratory Chemical Inventory Validation** | Hazard class tracking, storage capacity (MAQ) verification, pair-wise chemical incompatibility safety matrix. |
| **3** | **Academic Timetable Conflict Detection** | Interval overlap algorithms, back-to-back session validity, student schedule clash & room double-booking detection. |
| **4** | **University Scholarship Allocation System** | Multi-attribute filtering (aggregate %, cutoff marks, attendance, income limits), multi-key tie-resolution sorting. |
| **5** | **Campus Event Financial & Break-Even Planning** | Fixed vs. variable cost accounting, sponsorship shortfall analysis, Cost-Volume-Profit (CVP) break-even participant calculation. |
| **6** | **Railway Fare & Reservation System** | Distance slab pricing, travel class multipliers, age concessions (child/senior), time-dependent cancellation penalty logic. |
| **7** | **Attendance Recovery Computation System** | Current attendance tracking, minimum consecutive class recovery calculation to reach 75% eligibility, debarment prediction. |
| **8** | **ATM Transaction Sequence Simulation** | Stateful ledger processing, daily withdrawal limit enforcement, overdraft prevention, deposit/withdrawal error handling. |
| **9** | **Multi-Product Shopping Budget Constraint** | Category discount handling, budget overflow detection, priority-based (essential vs. luxury) greedy item reduction plan. |
| **10** | **Student Email & Identifier Validation** | Regex syntax parsing, malformed separator detection, department/year bounds checking, fine-grained error diagnostic reporting. |

---

## 🛠 Project Details & Module Specifications

### 1. Progressive Electricity Billing and Comparative Analysis System
Calculates energy charges using progressive slabs (Tier 1: 0–100 kWh, Tier 2: 101–300 kWh, Tier 3: >300 kWh). Automatically computes fuel surcharges (5%), regulatory taxes (12%), and prompt payment rebates (3%). Includes a multi-month comparative analyzer that flags unusual consumption spikes exceeding 25%.

### 2. Laboratory Chemical Inventory Validation System
Audits chemical storage setups against maximum allowable quantities (MAQ) and hazard safety matrices. Detects dangerous co-locations in storage cabinets (e.g., Flammables + Oxidizers, Acids + Bases, Water-Reactives) to ensure laboratory safety compliance.

### 3. Timetable Conflict Detection & Optimization System
Parses course schedules, days, and time slots into minute-based intervals ($[\text{start\_min}, \text{end\_min}]$). Utilizes interval overlap math $\max(S_1, S_2) < \min(E_1, E_2)$ to instantly identify student timetable clashes and room double-bookings.

### 4. University Scholarship Allocation & Tie-Resolution System
Filters applicants across four core criteria: minimum aggregate score (75%), subject cutoffs (60%), attendance (75%), and family income limits (₹8,00,000). Resolves rank ties deterministically using multi-key lexicographical sorting (Income $\rightarrow$ Attendance $\rightarrow$ Subject Scores).

### 5. Campus Event Financial Planning & Break-Even System
Consolidates venue, equipment, catering, and transport costs. Determines unit contribution margins ($P - VC$) and applies ceiling functions to compute the exact break-even attendee headcount needed to avoid budget deficits.

### 6. Railway Fare and Reservation Calculator System
Computes multi-passenger ticket fares considering distance slabs, class multipliers (Sleeper, 3A, 2A, 1A), reservation/superfast fees, age-based concessions (Infant, Child, Senior Citizen), and lead-time cancellation refund policies (>48h, 12–48h, <12h).

### 7. Attendance Recovery Computation System
Evaluates student eligibility against a 75% threshold. Uses the ceiling recovery formula $x = \lceil (T \cdot C - A) / (1 - T) \rceil$ to calculate the minimum consecutive classes needed to achieve exam eligibility and predict debarments.

### 8. ATM Transaction Sequence Simulation System
Processes a sequential stream of financial transactions while maintaining ledger integrity. Enforces single-transaction caps, daily cumulative withdrawal limits, overdraft protections, and generates detailed audit logs.

### 9. Multi-Product Shopping Budget Constraint System
Evaluates shopping baskets under hard budget ceilings. Applies product category discounts and uses a greedy reduction heuristic based on item priority ranks (Priority 1: Essential to Priority 3: Luxury) to trim items when budget overruns occur.

### 10. Student Email and Identifier Validation System
Enforces institutional grammar for email addresses (`user@domain.edu`) and registration identifiers (`REG-YYYY-DEPT-XXX`). Reports exact diagnostic errors including malformed separators, invalid character groups, range overflows, and missing components.

---

## 📁 Repository Structure

```text
├── electricity_billing.py          # Project 1: Electricity Billing System
├── chemical_inventory.py           # Project 2: Chemical Inventory Validator
├── timetable_validator.py          # Project 3: Timetable Conflict Detector
├── scholarship_allocator.py        # Project 4: Scholarship Allocation System
├── event_financial_planner.py     # Project 5: Campus Event Financial Planner
├── railway_fare_calculator.py     # Project 6: Railway Fare Calculator
├── attendance_recovery.py          # Project 7: Attendance Recovery Calculator
├── atm_simulation.py               # Project 8: ATM Transaction Simulator
├── shopping_budget_optimizer.py    # Project 9: Shopping Budget Optimizer
├── student_validator.py           # Project 10: Student Email & ID Validator
└── README.md                       # Repository Documentation
```

---

## 🚀 Execution & Usage

To run any individual module, execute the corresponding Python script using Python 3.13+:

```bash
# Run Electricity Billing System
python electricity_billing.py

# Run Chemical Inventory Validator
python chemical_inventory.py

# Run Railway Fare Calculator
python railway_fare_calculator.py
```

---

## 📌 Standard 11-Section Case Study Structure

Each case study in this repository is structured into the following 11 standardized technical sections:

1. **Problem Statement**
2. **Objectives**
3. **Assumptions**
4. **Mathematical & Logic Formulation**
5. **System Flowchart**
6. **Algorithm**
7. **Pseudocode**
8. **Python Source Code**
9. **Test Cases & Validation Matrix**
10. **Output Screenshots / Terminal Audit Results**
11. **Conclusion & Key Findings**
