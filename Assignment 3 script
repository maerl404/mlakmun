# GitHub Link: https://github.com/maerl404/Acenet-
#!/bin/bash
#SBATCH --job-name=habit-report
#SBATCH --time=00:05:00
#SBATCH --cpus-per-task=1
#SBATCH --mem=1G
# If the cluster asks for an account, add: #SBATCH --account=YOUR_ACCOUNT

# Load Python
module load python

# Make a virtual environment on the node and install asteval
virtualenv --no-download $SLURM_TMPDIR/env
source $SLURM_TMPDIR/env/bin/activate
pip install --no-index --upgrade pip
pip install --no-index asteval

# Run the script
python Project-HPC-mlakmun.py
