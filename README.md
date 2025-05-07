# Simulating a LoRaWAN Style Mesh Network Using Containers

## Overview
This project contains multiple LoRAWAN implementations and analysis tools. It includes Docker setups, Minikube configurations, and scripts to start different versions of the LoRAWAN network.

## Prerequisites
- Docker and Docker Compose installed
- Minikube installed 
- Python
- Bash shell to run shell scripts

## How to Run

### Starting Different Versions
- Use the scripts `start_all_versions.sh` or `start_two_versions.sh` in the root directory to start multiple versions of the LoRAWAN network.
- 
### Using Terminal

1. For running two main version of LoRAWAN Implementation (Docker and minikube)
chmod +x start_two_versions.sh
./start_two_version.sh <br>
2. For running all 4 version of LoRAWAN Implementation
chmod +x start_all_versions.sh
./start_all_versions.sh

### Running Python Scripts
- Creating of Virtual Environment is needed for plot creations and graph (start_*_versions does for you)<br>
- Python scripts AllComparision.py is run from within shart_*_versions script for analysis.

## Comparision Plots and Visual analysis
- Once start_*_version is ran, It automatically fetches the summay of metrics and stores in the root directry and it can be found under comparision_plots dir.

- Additionally for each version, All the plots related to metrics is stored under Report*_LoRAWAN_* directory
- Summary text file is stored in Summary_LoRAWAN_*

##

## Logs and Ignored Files
- All `collected_logs` directories are ignored in git.
- Python virtual environments (`venv`) are also ignored.

## Additional Notes
- Ensure you have the necessary permissions to run Docker and Kubernetes commands.
- Modify configuration files as needed for your environment.
