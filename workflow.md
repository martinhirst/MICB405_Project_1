
# Welcome to MICB405 Project 1: Epigenomic Data Analysis <a id="welcome"></a>

In this hands-on project you will work in teams to analyze the epigenetic state changes in the genomes of murine T-cells before (Naive T-cell) and following (Primary T-cell) influenza challenge.  We will focus our analysis on a histone modification that is associated with [active regulatory states](https://www.nature.com/articles/nrg3682) in mammalian genomes.  As you work through this project as a team it is highly recommended that you select one member of the team to run the BWA (mem) alignments and that you use one user account to demonstrate that the steps have completed successfully (see below for grading scheme).   

The workflow for this project can be found [here](https://github.com/martinhirst/micb405_project_1/blob/master/workflow.jpeg).

The (recommended) tools that you will working with to complete this project include:

1.  [BWA](https://github.com/lh3/bwa) 
2.  [SAMBAMBA](http://lomereiter.github.io/sambamba/)
3.  [MACS2](https://github.com/taoliu/MACS)
4.  [bedtools](http://bedtools.readthedocs.io/en/latest/)
5.  [GREAT](http://great.stanford.edu/public/html/index.php)
6.  [UCSC Genome Browser](https://genome.ucsc.edu/)

You may wish to explore other tools available to you on the orca docker that can be found through 'brew list' or can be found [here](https://github.com/bcgsc/orca/blob/master/versions.tsv).

Datasets for this project have been uploaded to the orca docker here:

mhirst@mhirst-ORCA:/home/micb405/data/project_1$ ls
CD4_Naive_Input_R1.fq

CD4_Primary_Input_R1.fq

CD4_Naive_Input_R2.fq

CD4_Primary_Input_R2.fq

CD4_Naive_H3K27ac_R1.fq

CD4_Primary_H3K27ac_R1.fq  

CD4_Naive_H3K27ac_R2.fq

CD4_Primary_H3K27ac_R2.fq  

These are paired-end 125 nt reads.  Curious about quality - you should be - use [FASTQC](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/).

NOTE:  When you are running commands that take a significant time to complete (for example BWA) you should write a simple [BASH script](http://tldp.org/LDP/Bash-Beginners-Guide/html/sect_02_01.html) and use [nohup](https://en.wikipedia.org/wiki/Nohup) to ensure your job does not terminate if your terminal disconnects.  The alignment step has benchmarked at 12-14hrs - so start this soon - the remaining steps should complete within 15mins.

The project will be conducted over 3 classes and 2 tutorials:

1. Nov. 2nd, 2017 (class):   Introduction to the topic area and the datasets
2. Nov. 3rd, 2017 (tutorial):  Team work with TAs
3. Nov. 7th, 2017 (class):   Team work with TAs and Instructors
4. Nov. 9th, 2017 (class):  Team presentations
5. Nov. 10th, 2017 (tutorial):  Report Due


The project will be assessed based on the following criteria:

1)	Completion at different stages of the [workflow](https://github.com/martinhirst/micb405_project_1/blob/master/workflow.jpeg). Outputs in correct format and directory structure logical (10%)

2)	Written Report (70-90%).  The written report should conform to following structure:
a.  Abstract (250 words)
b.  Introduction (500-1000 words)
c.  Methods (1000-2000 words including workflow, directory structure, commands with parameter selection rationale in written report)
d.  Results (1000-2000 words), 
e.  Unlimited figures, tables and references.

3)	Oral presentation (20%).  10 min presentation should follow general structure of the written report with emphasis on results.


