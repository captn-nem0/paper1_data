# Raw Simulation Data Repository

This repository contains raw data files used for generating figures in the study.  
All files are provided in compressed `.zip` format and contain only simulation/output data (no source code).

---

# Repository Structure

## fig_1_2

This directory contains data related to Figures 1 and 2.

### Folder Structure

There are two main folders:

- `wi_virtual` → with virtual particles
- `wo_virtual` → without virtual particles

Inside each of these folders, there are three subfolders corresponding to different boundary conditions:

- `Bounceback`
- `Stochastic`
- `Hybrid`

Each boundary-condition folder contains four datasets:

- Temperature data
- Density data
- Flow data
- Temperature evolution data (`temp_evolv.dat`)

### temp_evolv.dat

- Data provided up to **1,000,000 iterations**
- Values stored every **1000 iterations**
- Data includes temperature values for every layer of the simulation box

---

# fig_3

This folder contains four files:

- `x_vel.dat` → x-axis values for translational velocity distribution
- `hist_vel.dat` → y-axis values for translational velocity distribution
- `x_ang.dat` → x-axis values for angular velocity distribution
- `hist_ang.dat` → y-axis values for angular velocity distribution

### Bin Widths

- Angular velocity case: `bin_width = 0.0045`
- Translational velocity case: `bin_width = 0.0069`

---

# fig_4_8

This folder contains:

- `ke_shell_pasv.dat` → data for Figure 4
- `ke_shell_actv.dat` → data for Figure 8

### Data Format

- Data is presented for **20 shells**
- Rows correspond to different iterations:

| Rows | Iteration |
|------|------------|
| 1–20 | \(10^0\) |
| 21–40 | \(10^1\) |
| ... | ... |
| 121–140 | \(10^7\) |

Each row contains shell-wise values for a particular iteration.

---

# fig_6

This folder contains four files:

- `x.dat` → x-axis values for active colloid
- `hist.dat` → y-axis values for active colloid
- `x_passive.dat` → x-axis values for passive colloid
- `hist_passive.dat` → y-axis values for passive colloid

### Bin Width

- Active/passive case: `bin_width = 0.0084`

---

# fig_7

This folder contains a single file with:

- **7 columns**
- **5 rows**

### Rows correspond to:

\[
v_a = 0.04,\ 0.08,\ 0.1,\ 0.2,\ 0.4
\]

### Columns correspond to:

\[
\theta = 300,\ 270,\ 240,\ 180,\ 120,\ 90,\ 60
\]

---

# fig_9

This folder contains three files:

- MSD data
- VAC data
- AVAC data

### File Format

Each file contains four columns:

1. Iteration number
2. Value along x-direction
3. Value along y-direction
4. Value along z-direction

---

# fig_10_12_13_14_15_inward

Contains flow-profile data for different values of \(\theta\) for the inward-pumping case.

### Files

- `index.dat`
  - Contains position coordinates:
    - x
    - y
    - z

- Flow files
  - Contain x, y, and z components of flow corresponding to the coordinates in `index.dat`

---

# fig_10_12_13_14_15_outward

Contains flow-profile data for different values of \(\theta\) for the outward-pumping case.

### Files

- `index.dat`
  - Contains x, y, and z coordinate positions

- Flow files
  - Contain x, y, and z components of flow corresponding to `index.dat`

---

# fig_11

Contains flow-profile data for both inward and outward cases.

### Files

- `index.dat`
  - Contains x, y, and z coordinate positions

- Flow files
  - Contain x, y, and z components of flow corresponding to `index.dat`

---

# Notes

- All files contain raw numerical simulation data.
- No source code is included in this repository.
- File names are preserved exactly as used during data generation and analysis.
