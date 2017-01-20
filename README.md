#AsmSlurm

By Karin Lagesen | @karinlag

##About

This repo contains code intended to take fastq files through quality control, trimming
and assembly. The code is created to run under the slurm queueing system as found
on abel.uio.no.

###Software dependencies

The following software is used in this pipeline:

- fastqc: calculates quality measures for fastq files
- trimmomatic: does quality trimming and end trimming on fastq files
- SPAdes: genome assembly software


###Structure

There are several steps in this pipeline:

1. fastqc is run on all input files
  * Summary qualities are subsequently calculated
1. trimmomatic is run on all input files
1. fastqc is again run on the trimmomatic results
  * Summary qualities are subsequently calculated
1. spades is run on all input files
  * Statistics is calculated on the resulting assemblies
   
   



