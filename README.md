##   bruteforce
#### Oktober 2022, Snorre Flo
The following code has been used for processing large quantities of mixed sample sequencing data for prey studies in small Arctic copepods. The scripts take .fastq-files with multiplexed samples distinguished by oligotags, and returns a .txt-table with zero-radius OTUs (rows), associated taxonomy (PR2, columns) and sample counts (columns). 

NB! Manual considerations and modifications to code are needed to implement scripts in other pipelines. 

The brute_#.txt scripts do the following processing:
* brute_1.txt - pairing, quality-filtering, demultiplexing, length-filtering
* brute_2.txt - streamlining by cutting unnecessary variables, splitting by sample
* brute_3.txt - dereplicating, denoising, chimeric removal
* brute_4.txt - concatenating samples, re-dereplicating, taxonomic assignment and export

Additional scripts for quality checking and generating database for taxonomic assignment:
* fastqc_stats_jobscript.txt
* PR2_v4.14.0_db_prep.txt

Software/database and versions used:
* FastQC/0.11.9 (https://github.com/s-andrews/FastQC, https://www.bioinformatics.babraham.ac.uk/projects/fastqc/)
* BLAST+/2.8.1 (Altschul et al. 1990, Camacho et al. 2009, https://pubmed.ncbi.nlm.nih.gov/2231712/)
* OBITools/1.2.12 (Boyer et al. 2016, https://git.metabarcoding.org/obitools/obitools, https://pythonhosted.org/OBITools/introduction.html)
* VSEARCH/2.9.1 (Rognes et al. 2016, https://github.com/torognes/vsearch)
* Protist Ribosomal database (PR2)/4.14.0 (Guillou et al. 2013, https://pr2-database.org/)

