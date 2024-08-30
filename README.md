# Stage4: Statistical Analysis and Verification of Neuron Activations

**Required Inputs:**
1) config_files/ neuron_<neuron_id>_results_ecii_V2.txt
   
   (_Path: /homes/samatha94/ExAI_inputs_and_outputs/Stage1_Results/config_files_)
2) evaluation/neuron<neuron_id>_solution<solution_id>_evaluation_set.csv

   (_Path: /homes/samatha94/ExAI_inputs_and_outputs/Stage3_Results/evaluation_)
3) verification/neuron<neuron_id>_solution<solution_id>_verification_set.csv

   (_Path: /homes/samatha94/ExAI_inputs_and_outputs/Stage3_Results/verification_)


**Expected Outputs:**                  (_Path: /homes/samatha94/ExAI_inputs_and_outputs/Stage4_Results_)
1) evaluation_combined.xlsx
2) verification_combined.xlsx

**Instructions to Set Up the Environment and Run the Python Script:**
1) Install Python 3.11.5

   Ensure Python 3.11.5 is installed on your system by executing below command

   python --version
   
3) Set Up a Virtual Environment

   Install virtualenv if it is not already installed
    
    pip install virtualenv
   
5) Create a virtual environment named 'venv'

   python -m venv venv
   
7) Activate the Virtual Environment

   On macOS/Linux:

   source venv/bin/activate

   On Windows:

   venv\Scripts\activate
   
9) Install Required Python Packages:

   pip install tensorflow Pillow scipy pandas scikit-learn gdown
   
11) Run the Python Script

      python main.py

**Steps to Run the Script on BeoCat:**

**Bash file name:** job_stage4.sh

**Bash Script:** https://github.com/Samatha1994/Bash_scripts/blob/main/job_stage4.sh

**Bash Command to kick off the job:** sbatch job_stage4.sh

**Bash command to check the status of the job:** 

sacct --format=JobID,JobName,State,ReqMem,MaxRSS,Start,End,TotalCPU,Elapsed,NCPUS,NNodes,NodeList --jobs= <job_id>

**Log file:** my_job_output_<job_id>.txt (Path: /homes/samatha94/)

**Bash Command to cancel the job:** scancel job_id


