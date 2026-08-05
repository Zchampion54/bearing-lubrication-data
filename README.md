# Bearing Lubrication Experimental Data

## Overview
The dataset contains vibration signals collected under normal lubrication and insufficient lubrication conditions at different rotational speeds.

## Dataset structure

```text
experimental_data/
├── normal_lubr/
│   ├── Fr20N700.csv
│   ├── Fr20N800.csv
│   ├── ...
│   └── Fr20N1800.csv
│
└── insufficient_lubr/
    ├── 0g20kgN700.csv
    ├── 0g20kgN800.csv
    ├── ...
    └── 0g20kgN1800.csv
```

## Lubrication conditions

### Normal lubrication

The `normal_lubr` folder contains experimental data collected under the normal lubrication condition.

The filenames range from `Fr20N700.csv` to `Fr20N1800.csv`. The numerical suffix indicates the rotational speed in revolutions per minute.

### Insufficient lubrication

The `insufficient_lubr` folder contains experimental data collected under the insufficient lubrication condition.

The filenames range from `0g20kgN700.csv` to `0g20kgN1800.csv`. The numerical suffix indicates the rotational speed in revolutions per minute.

## CSV data format

Each CSV file contains [insert number] columns:

  1. Column 1: [Time]
2. Column 2: [experimental data]


The sampling frequency was [200K] Hz.

The duration of each recording was approximately [15] s.

## Experimental conditions

* Rotational speed range: 700–1800 r/min
* Lubrication conditions: normal lubrication and insufficient lubrication
* Applied load: [20kg]
* Sensor type: [SPM sensor]
* Sampling system: [Dewesoft]
* Sampling frequency: [200K] Hz

## Data access

The experimental data are stored using Git Large File Storage because individual CSV files exceed the standard GitHub file-size limit.

Users downloading the repository through Git should install Git LFS before cloning:

```bash
git lfs install
git clone [insert repository address]
```

