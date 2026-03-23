# Environment Setup for CS 7150 on the Explorer cluster

## Quick Start

First of all, log into the Explorer cluster via either commandline or OOD (Open OnDemand). Request a node, for example, by running 
```bash
srun -p courses-gpu --gres=gpu:p100:1 --time=01:00:00 --pty bash
```

Once the resources are allocated, you will be in a terminal running in the **computing node**. Run the following command then.
```bash
bash setup.sh
source activate cs7150
```

This creates a conda environment with Python, NumPy, Matplotlib, Jupyter, and
PyTorch (with CUDA 11.8 support). The setup takes a few minutes.

After the setup, you are ready to work on PA2 in the OOD portal.