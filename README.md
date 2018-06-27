# atacseq_pipeline

This repository contains files for analysis of samples 67S and 67V in the ATAC-seq pipeline.

"atac_seq_pipeline_1.r" is an R script containing only a vector of all the 8 filenames for the two samples. Because these samples were paired-end, names are included for foward and reverse reads in addition to both of the two sequencing runs. "ATAC_67(S,V)_reseq1_(1,2).fq.gz" should be analyzed together, while ATAC_"HMTB067(S,V)_(1,2).fq.gz" should be analyzed together.

"pipelineSubmit.sh" is a shell script that runs "pipeline_v2_ex.r"

"pipeline_v1.py" creates a list of the 8 filenames listed in "atac_seq_pipeline_1.r" as well as a skelton commented code for the analysis pipeline. 

"pipeline_v1_ex.r" and "pipeline_v1_ex.r" are versions of the pipeline for two specific file pairs, namely the first sequencing run (ATAC_) for 67S and 67V, respectively. The former example file contains the entire bsub commands to be run on the PMACS cluster. 