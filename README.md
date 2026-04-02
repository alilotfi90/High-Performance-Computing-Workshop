# High Performance Computing Workshop

**Agronomic Crop Imaging Lab**  
Department of Plant Sciences, University of Saskatchewan  
*Ali Lotfi*

---

<p align="center">
  <img src="universalAI.png" alt="AI and HPC for Agricultural Research" width="80%"/>
</p>

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

1. **What Is an HPC Cluster?** — nodes, login vs compute, why HPC matters for imaging research
2. **Logging In via SSH** — connecting from Windows, Duo authentication, reading the prompt
3. **Finding Your Way Around** — `pwd`, `ls`, `cd`, absolute vs relative paths, filesystem layout
4. **Creating, Moving, and Deleting Files** — `nano`, `mv`, `cp`, `rm`, chaining commands
5. **Wildcards, Redirection, and Pipes** — `*`, `>`, `|`, `grep`, compression with `tar` and `gzip`
6. **Shell Scripts, Variables, and Loops** — writing `.sh` scripts, variables, for loops, `chmod`
7. **Submitting Jobs with SLURM** — job scripts, monitoring, time limits, resource tuning
8. **Loading Software with Modules** — `module load`, version pinning, reproducibility
9. **Running Python on the Cluster** — virtual environments, pip, batch Python jobs
10. **Transferring Files** — `scp`, `dos2unix`, `tar`, `rsync` from Windows
11. **Running GPU Jobs** — finding GPUs with `sinfo`, requesting H100 slices, training a CNN

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
