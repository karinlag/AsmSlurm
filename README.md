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


