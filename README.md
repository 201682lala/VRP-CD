# Vehicle routing problem with collective drones in post-disaster relief logistics

This repository provides the datasets, solution code, and detailed computational results accompanying the paper *Vehicle routing problem with collective drones in post-disaster relief logistics*. The code includes the mixed-integer linear programming (MILP) model solved with Gurobi and the branch-and-price (BP) algorithm.

The Excel workbook `Detailed Computational_Results Tables.xlsx` contains the detailed computational results.

## Requirements

Python, NumPy, and Gurobi with a valid license. Install the required packages with:

```bash
pip install -r requirements.txt
```

## Usage

Run the following commands from the `Solver` directory.

Solve the MILP model with Gurobi:

```bash
python Main_BP.py --name 3_0.1_c_e --method solver --time-limit 3600
```

Run the BP algorithm:

```bash
python Main_BP.py --name 3_0.1_c_e --method bp --time-limit 3600
```

Replace `3_0.1_c_e` with the desired instance name from `data/`. The time limit is specified in seconds.

