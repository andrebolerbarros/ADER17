## ADER17 ##

4-day course at Instituto Gulbenkian de Ciência

Official course page

http://gtpb.igc.gulbenkian.pt/bicourses/ADER17/


# Overview

High-throughput technologies allow us to detect transcripts present in a cell or tissue. This course covers practical aspects of the analysis of differential gene expression by RNAseq. Participants will be presented with real world examples and work with them in the training room, covering all the steps of RNAseq analysis, from planning the gathering of sequence data to the generation of tables of differentially expressed gene lists and visualization of results. We we will also cover some of the initial steps of secondary analysis, such as functional enrichment of the obtained gene lists.


# Target Audiences

Life Scientists who want to be able to use NGS data to evaluate gene expression (RNAseq). Computational researchers that wish to get acquainted with the concepts and methodologies used in RNAseq are also welcome. Participants are encouraged to bring their own data and will have the opportunity to apply the concepts learned in the course. 


# Pre-requisites

Familiarity with elementary statistics and a few basics of scripting in R will be helpful.

Please have a look at the following resources and gauge your ability to use R in statitics at the basic level:
- http://blog.revolutionanalytics.com/2012/12/coursera-videos.html
- http://bitesizebio.com/webinar/20600/beginners-introduction-to-r-statistical-software

Basic Unix command line skills, such as being able to navigate in a directory tree and copy files. See, for example, "Session 1" of the Software Carpentry training for a Unix introduction (http://bioinformatics-core-shared-training.github.io/shell-novice/). 


# Learning Objectives

At the end of the course, we expect every participant to be able to:
- Have a broad overview of the steps in the analysis of RNA-Seq differential expression experiments
- Assess the general quality of the raw data from the sequencing facility
- Do simple processing operations in the raw data to improve its quality
- Generate alignments against a reference genome
- Assess the general quality of the alignments and detect possible problems
- Generate tables of counts using the alignment and a reference gene annotation
- Generate lists of differentially expressed genes, at least for a simple pairwise comparison
- Perform simple functional enrichment analysis and understand the concepts behind them

For this, we will provide small example datasets that students can use to learn. 

Students are encouraged to bring their own data and try some of the concepts they learned. For simple cases, participants may even be able to generate the complete analysis on their own data.


# TODO

Pedro's suggestions:

    Define the overall learning objectives: DONE
    Break down in units (sub-objectives) that can be assigned to instructors: DONE

    Identify learning outcomes for each unit.
    For each outcome design an exercise
    For each exercise identify the short lecture needed and the materials

- Have a broad overview of the steps in the analysis of RNA-Seq differential expression experiments
	-- NGS technologies have revolutionized sequencing
		--- Illumina is (still) the most prevalent technology
		--- There are different sequencing options and each has consequences for analysis
		--- Technology evolves fast, you need to know what is done to be able to interpret
	-- Steps in RNA-Seq differential gene expression analysis: 
		--- QC of Raw Data; 
		--- Preprocessing of Raw Data (if needed); 
		--- Alignment of processed reads to reference genome; 
		--- QC of Aligments (optional); 
		--- Generate table of counts of genes/transcripts
		--- QC of count table
		--- Preprocessing of count table
		--- Differential Analysis tests
		--- Post-analysis: Functional Enrichment

- Assess the general quality of the raw data from the sequencing facility
	-- NGS data usually comes in fastq files
	-- Fastq files store sequencing data as text files
	-- Each sequencing read is represented as 4 lines of text which includes sequence and quality
	-- software like FastQC can be used to automatically process fastq and produce QC reports
	-- QC reports will inform you of the general quality of your reads, and presence of sequence bias

- Do simple processing operations in the raw data to improve its quality
	-- Use tools such as seqtqk and trimmomatic to remove low quality bases from your reads
	-- Use tools such as cutadapt to remove adaptors and other artefactual sequences from your reads

- Generate alignments of processed reads against a reference genome
	-- Sources of reference genomes: Ensembl; NCBI; (be wary of versions)
	-- Preprocessing of the reference genome for aligment
	-- Alignment software: tophat2/hisat2; bwa mem
	-- Running an alignment
	-- 
	
- Assess the general quality of the alignments and detect possible problems
- Generate tables of counts using the alignment and a reference gene annotation
- Generate lists of differentially expressed genes, at least for a simple pairwise comparison
- Perform simple functional enrichment analysis and understand the concepts behind them

    Compose a schedule, spreading moments of wrap-up, feedback, Q&A, etc. 



