# High Performance Computing Workshop

**Agronomic Crop Imaging Lab**  
Department of Plant Sciences, University of Saskatchewan  
*Ali Lotfi*

---

## Overview

This repository contains hands-on tutorial materials for the **Fir HPC cluster** (Digital Research Alliance of Canada). The tutorial covers everything a lab member needs to go from first SSH login to running deep learning models on NVIDIA H100 GPUs.

Every command in these materials was tested live on Fir.

---

## Contents

| File | Description |
|------|-------------|
| `HPC_WorkShop.pdf` | Full tutorial document — read this |
| `fir-codes-and-commands.txt` | All commands and code for copy-paste (avoids PDF spacing issues) |

---

## What You Will Learn

1. **Submitting Jobs with SLURM** — job scripts, monitoring, time limits, resource tuning
2. **Loading Software with Modules** — `module load`, version pinning, reproducibility
3. **Transferring Files** — `scp`, `dos2unix`, `tar`, `rsync` from Windows
4. **Running Python on the Cluster** — virtual environments, pip, batch Python jobs
5. **Running GPU Jobs** — finding GPUs with `sinfo`, requesting H100 slices, training a CNN

---

## Prerequisites

- An active [Digital Research Alliance of Canada](https://alliancecan.ca) account
- Your PI's allocation group (e.g. `def-yourPI_cpu` / `def-yourPI_gpu`)
- Windows with PowerShell or Command Prompt
- Duo Mobile app for two-factor authentication

---

## Quick Start

```bash
# Connect to Fir
ssh yourUsername@fir.alliancecan.ca

# Create your working directory
cd ~/scratch
mkdir hpc-tutorial
cd hpc-tutorial
```

Then open `HPC_WorkShop.pdf` and work through the sections in order. Use `fir-codes-and-commands.txt` to copy-paste commands without formatting issues.

---

## Cluster Details

| Resource | Value |
|----------|-------|
| Cluster | Fir (`fir.alliancecan.ca`) |
| Scheduler | SLURM |
| GPUs | NVIDIA H100 80GB (MIG-partitioned) |
| CPU account | `def-kanj241_cpu` |
| GPU account | `def-kanj241_gpu` |

---

## Contact

**Ali Lotfi**  
Agronomic Crop Imaging Lab  
Department of Plant Sciences  
University of Saskatchewan  
GitHub: [@alilotfi90](https://github.com/alilotfi90)
