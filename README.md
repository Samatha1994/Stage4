# Stage4: Statistical Analysis and Verification of Neuron Activations

**Required Inputs:**
1) config_files/ neuron_<neuron_id>_results_ecii_V2.txt                      (Path: /homes/samatha94/ExAI_inputs_and_outputs/Stage1_Results)
2) evaluation/neuron<neuron_id>_solution<solution_id>_evaluation_set.csv     (Path: /homes/samatha94/ExAI_inputs_and_outputs/Stage3_Results/evaluation)
3) verification/neuron<neuron_id>_solution<solution_id>_verification_set.csv (Path: /homes/samatha94/ExAI_inputs_and_outputs/Stage3_Results/verification)


**Expected Outputs:**                  (Path: /homes/samatha94/ExAI_inputs_and_outputs/Stage4_Results)
1) evaluation_combined.xlsx
2) verification_combined.xlsx
   




**Bash file name:** job_stage4.sh

**Bash Command to kick off the job:** sbatch job_stage4.sh

**Bash command to check the status of the job:** 

sacct --format=JobID,JobName,State,ReqMem,MaxRSS,Start,End,TotalCPU,Elapsed,NCPUS,NNodes,NodeList --jobs= <job_id>

**Log file:** my_job_output_<job_id>.txt (Path: /homes/samatha94/)

**Bash Command to cancel the job:** scancel job_id


