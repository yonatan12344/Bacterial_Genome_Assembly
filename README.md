
# Bacterial_Genome_Assembly
quick bacterial genome assembly from short illumina raw reads.
# Test Data
The test data is actually just a fastQ file of raw short read illumina data, from the following SRA, SRR21201071, which was a sequencing effort for Pseudomonas aeruginosa . I used sratools to dump the fastq file, compressed it, and used zcat to extract the first 10000 lines of the forward and reverse read. That then became the test data, in order to showcase the parallel processing capability of my pipeline, I copied these two files, and altered the names adding them to the test data.
### Test Data names and Explanations
* SRR21201071_mini_1.fastq.gz: zcat of first 10k lines of SRR21201071 forward fastQ file
* SRR21201071_mini_2.fastq.gz: zcat of first 10k lines of SRR21201071 reverse fastQ file
* SRR21201071_mini_copy_1.fastq.gz: copy of SRR21201071_mini_1.fastq.gz file
* SRR21201071_mini_copy_2.fastq.gz: copy of SRR21201071_mini_2.fastq.gz file
# Requirments
This project is for Biol 7210.
This code was tested for x86, on Linux Mint. Nextflow was run through a conda enviornemnt, and package managment within the pipeline is handled by conda.The conda version used to run nextflow was, conda 26.1.1 , the nextflow version within that conda environment used to run nextflow was nextflow version 25.10.4.11173 . 
# Workflow Diagram
<img width="4624" height="3472" alt="PXL_20260421_135844734" src="https://github.com/user-attachments/assets/654f47c1-c88e-40ee-8ebd-5ee7c9fd0ef3" />

