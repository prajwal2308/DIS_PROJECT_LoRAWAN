# LoRAWAN Project

## Overview
This project contains multiple LoRAWAN implementations and analysis tools. It includes Docker setups, Minikube configurations, and scripts to start different versions of the LoRAWAN network.

## Prerequisites
- Docker and Docker Compose installed (for Docker-based setups)
- Minikube installed (for Kubernetes-based setups)
- Python 3.x installed (for running Python scripts)
- Bash shell to run shell scripts

## How to Run

### Using Docker
1. Navigate to the `LoRAWAN_Docker` directory:
   ```bash
   cd LoRAWAN_Merge/LoRAWAN_Docker
   ```
2. Start the Docker containers:
   ```bash
   docker-compose up --build
   ```
3. Use the provided scripts like `start.sh` to manage the Docker setup.

### Using Minikube
1. Navigate to the `LoRAWAN_minikube` directory:
   ```bash
   cd LoRAWAN_Merge/LoRAWAN_minikube
   ```
2. Deploy the mesh using the provided YAML files:
   ```bash
   kubectl apply -f mesh-deployment.yaml
   kubectl apply -f mesh-headless-service.yaml
   ```
3. Use the `start.sh` script to start the Minikube setup.

### Running Python Scripts
- Python scripts like `analyze_mesh.py` are available in various directories for analysis.
- Run them using:
  ```bash
  python3 analyze_mesh.py
  ```

### Starting Different Versions
- Use the scripts `start_all_versions.sh` or `start_two_versions.sh` in the root directory to start multiple versions of the LoRAWAN network.

## Logs and Ignored Files
- All `collected_logs` directories are ignored in git.
- Python virtual environments (`venv`) are also ignored.

## Additional Notes
- Ensure you have the necessary permissions to run Docker and Kubernetes commands.
- Modify configuration files as needed for your environment.
