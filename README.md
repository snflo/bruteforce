# bruteforce
The following code has been used for processing and analysing large quantities of mixed sample sequencing data for prey analysis of small Arctic copepods. Manual considerations are needed to implement scripts in other pipelines. 

brute_# scripts perform bioinformatic processing of sequences
* brute_1.txt - parallelized, pairing, quality-filtering, demultiplexing, length-filtering
* brute_2.txt - streamlining by cutting unnecessary variables, splitting by sample
* brute_3.txt - dereplicating, denoising, chimeric removal
* brute_4.txt - concatenating samples, re-dereplicating, taxonomic assignment and export

Additional scripts for quality checking and generating database for taxonomic assignment
* fastqc_stats_jobscript.txt
* PR2_v4.14.0_db_prep.txt

Software/version used:
* FastQC/0.11.9
* BLAST+/2.8.1
* OBITools/1.2.12
* VSEARCH/2.9.1

September 2022, Snorre Flo
---
